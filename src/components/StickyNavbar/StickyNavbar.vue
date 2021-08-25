<template>
    <div id="navbar">
        <div class="navbar-sub-main">
            <div class="navbar-link">
                <router-link to="/">
                    <h4>Home</h4>
                </router-link>
            </div>
            <div class="navbar-link">
                <router-link to="/about"><h4>About</h4></router-link>
            </div>
            <div class="navbar-link">
                <router-link to="/contact"><h4>Contact</h4></router-link>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'StickyNavbar',
     
        methods: {
            makeNavbarSticky() {
                let navbar = document.getElementById('navbar')
                let sticky = navbar.offsetTop

                if (window.pageYOffset >= sticky) {
                    navbar.classList.add('sticky')
                } else {
                    navbar.classList.remove('sticky')
                }
            }
        },
        mounted() {
            this.makeNavbarSticky()
        },
        created () {
            //Giving fake value to triger makeNavbarSticky function.
            window.pageYOffset = 300;
        },
    }
</script>

<style scoped>
    #navbar {
        width: 100%;
        height: 5vh;
        border-top: 1px rgb(131, 131, 131) solid;
        border-bottom: 1px rgb(131, 131, 131) solid;
        background: #2e2e27;
        display: flex;
        position: sticky;
        justify-content: center;
        align-items: center;
    }
    .navbar-sub-main {
        width: 45%;
        display: flex;
        justify-content: space-around;
        align-items: center;
    }
    .navbar-link {
        width: 150px;
        height: 3.5vh;
        background-color: rgb(85, 85, 85);
        border-radius: 30px;
        display: flex;
        justify-content: center;
        align-items: center;
        cursor: pointer;
    }

    a {
        color: rgb(197, 197, 197);
        text-decoration: none;
    }
    a:hover {
        transition: all 0.5s;
        color: white;
    }
    .sticky {
        position: fixed;
        top: 0;
        width: 100%;
        z-index: 500001;
    }
</style>
