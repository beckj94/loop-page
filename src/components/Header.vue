  <template>
    <div id="header">
        <div class="container">
            <div id="header-menu">
                <ul id="header-menu-list">
                    <li @click="toggleMenu()"><a href="#">about us</a></li>
                    <li @click="toggleMenu()"><a href="#">gallery</a></li>
                    <li @click="toggleMenu()"><a href="#">crew</a></li>
                    <li @click="toggleMenu()"><a href="#">kontakt</a></li>
                </ul>
                <button id="mobile-menu-button" @click="toggleMenu()">
                    <img src="/images/icons/menu.png">
                </button>
            </div>
            <div id="header-logo">
                <a href="/"><img src="/images/team-logo.png"></a>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Header',
     data(){
        return{
            menuOpened: false,
        }
    },
    methods: {
        toggleMenu() {
            document.getElementById('popup-backdrop').classList.toggle('opened')
            document.getElementById('header-menu-list').classList.toggle('opened')
        }
        // openMenu() {
        //     this.menuOpened = true
        //     document.getElementById('popup-backdrop').classList.add('opened')
        //     document.getElementById('header-menu-list').classList.add('opened')
        // },
        // closeMenu() {
        //     this.menuOpened = false
        //     document.getElementById('popup-backdrop').classList.remove('opened')
        //     document.getElementById('header-menu-list').classList.remove('opened')
        // }
    },
}
</script>