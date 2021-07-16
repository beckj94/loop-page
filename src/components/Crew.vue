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
                    <li>Show all</li>
                    <li>Trim</li>
                    <li>Tactics</li>
                    <li>Helmsman</li>
                </ul>
            </div>
            <div id="crew-list" class="row no-gutters">
                <div class="crew-tile col-12 col-sm-6 col-md-4 col-lg-3"
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
            <div class="d-flex align-items-center justify-content-center pt-4 pb-4">
                <button class="custom-btn btn-outline btn-white">Load more</button>
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
            crew: crewJson
        }
    }
}
</script>