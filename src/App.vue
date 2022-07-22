<template>
    <div id="app">
        <div class="top-banner-writing">
            <h1>Wireframe</h1>
        </div>
        <StickyNavbar />
        <CustomCarousels />
        <router-view />
    </div>
</template>
<script>
    import CustomCarousels from './components/CustomCarousels/CustomCarousels'
    import StickyNavbar from './components/StickyNavbar/StickyNavbar'

    export default {
        name: 'Home',
        components: {
            CustomCarousels,
            StickyNavbar
        },
        props: {}
    }
</script>
<style>
    #app {
        font-family: Avenir, Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
 
    }
    * {
        margin: 0;
        padding: 0;
    }
    .top-banner {
        width: 100%;
        height: 95vh;
        background-color: #2e2e27;
    }
    .top-banner-writing {
        height: 5vh;
        padding-left: 50px;
        padding-top: 50px;
        padding-bottom: 30px;
    }
    h1 {
        font-size: 3rem;
        text-align: start;
        color: #f1bd13;
    }
    @media only screen and (max-width: 1400px) {
        .top-banner {
            height: 75vh;
        }
    }
    @media only screen and (max-width: 1200px) {
        .top-banner {
            height: 67vh;
        }
    }
</style>
