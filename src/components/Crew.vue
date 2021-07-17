  <template>
    <div id="crew">
        <div id="clipped-top"></div>
        <div class="bg-black">
            <div class="container">
                <h1>Unser team</h1>
                <h3>Subtitle von unser team</h3>
                <div class="divider"></div>
            </div>
            <div id="filters">
                <ul>
                    <li @click="startLoadingFilter('all')" :class="{'active': activeFilter == 'all'}">Show all</li>
                    <li @click="startLoadingFilter('trim')" :class="{'active': activeFilter == 'trim'}">Trim</li>
                    <li @click="startLoadingFilter('tactics')" :class="{'active': activeFilter == 'tactics'}">Tactics</li>
                    <li @click="startLoadingFilter('helmsman')" :class="{'active': activeFilter == 'helmsman'}">Helmsman</li>
                </ul>
            </div>
            <div class="text-center"><span v-if="loading">Loading...</span></div>
            <div id="crew-list" class="row no-gutters" :class="{'loading': loading}">
                <div class="crew-tile col-12 col-sm-6 col-md-4"
                v-for="member in crew"
                :key="`crew-member-${member.name}`">
                    <div class="member-profile-image"
                    :style="`background-image: linear-gradient(black, black), url(${member.image})`">
                    </div>
                    <div class="member-data">
                        <div class="member-name">{{member.name}}</div>
                        <div>{{member.duties}}</div>
                    </div>
                </div>
            </div>
            <div class="d-flex align-items-center justify-content-center pt-5 pb-5">
                <button class="custom-btn btn-outline btn-white"
                @click="startLoadingMore()"
                v-if="!noMore"
                :disabled="loading">
                    <span v-if="!loading">Load more</span>
                    <span v-if="loading">Loading...</span>
                </button>
            </div>
        </div>
    </div>
</template>

<script>

import crewJson from '@/assets/sailor_team.json'

export default {
    name: 'Crew',
    data(){
        return{
            crew: [],
            perPage: 10,
            loading: false,
            noMore: false,
            activeFilter: 'all'
        }
    },
    methods: {
        getMembers(filterName = 'all') {
            this.crew = []
            switch (filterName) {
                case 'all':
                    this.activeFilter = 'all'
                    this.noMore = false
                    for(let i=0; i<10; i++) {
                        this.crew.push(crewJson[i])
                    }
                    break;
                case 'trim':
                    this.activeFilter = 'trim'
                    this.noMore = true
                    crewJson.forEach(element => {
                        element.duty_slugs.forEach(slug => {
                            if(slug == 'trim') {
                                this.crew.push(element)
                            }
                        })
                    })
                    break;
                case 'tactics':
                    this.activeFilter = 'tactics'
                    this.noMore = true
                    crewJson.forEach(element => {
                        element.duty_slugs.forEach(slug => {
                            if(slug == 'tactic') {
                                this.crew.push(element)
                            }
                        })
                    })
                    break;
                case 'helmsman':
                    this.activeFilter = 'helmsman'
                    this.noMore = true
                    crewJson.forEach(element => {
                        element.duty_slugs.forEach(slug => {
                            if(slug == 'helmsman') {
                                this.crew.push(element)
                            }
                        })
                    })
                    break;
            }
            this.loading = false
        },
        // load the next 10 if there are more
        loadMore: function() {

            let currentNumOfMembers = this.crew.length

            for(let i = 0; i <= this.perPage; i++) {
                if(typeof crewJson[i+currentNumOfMembers] !== 'undefined') {
                    this.crew.push(crewJson[i+currentNumOfMembers])
                } else {
                    this.noMore = true
                    break;
                }
            }

            this.loading = false
        },
        startLoadingMore() {
            this.loading = true
            setTimeout(
                function(){
                    this.loadMore()
                }
                .bind(this),
                1500
            )
        },
        startLoadingFilter(filterName) {
            this.loading = true
            setTimeout(
                function(){
                    this.getMembers(filterName)
                }
                .bind(this),
                1500
            )
        }
    },
    mounted() {
        this.getMembers()
        // for(let i=0; i<10; i++) {
        //     this.crew.push(crewJson[i])
        // }
    }
}
</script>