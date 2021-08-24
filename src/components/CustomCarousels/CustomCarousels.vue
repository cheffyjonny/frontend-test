<template>
    <div class="main">
        <vueper-slides slideContentOutside="bottom" :touchable="false" style="font-style: italic; color: white; line-height: 50px; font-size: 1.2rem; text-align: center">
            <vueper-slide v-for="(slide, i) in slides" :key="i" :title="slide.title" :content="slide.content" :image="slide.image" :link="slide.link"> </vueper-slide>
        </vueper-slides>
    </div>
</template>

<script>
    import { VueperSlides, VueperSlide } from 'vueperslides'
    import 'vueperslides/dist/vueperslides.css'

    export default {
        name: 'CustomCarousels',
        components: {
            VueperSlides,
            VueperSlide
        },
        data() {
            return {
                slides: [
                    {
                        title: 'Personal Portfolio',
                        content: '-This is a personal portfolio about `John Lee`.',
                        image: require('../../assets/PersonalPortfolio.png'),
                        link: 'https://cheffyjonny-personalportfolio.netlify.app'
                    },
                    {
                        title: 'Mine Sweeper',
                        content: '-This is one of the best old-school game in the world!',
                        image: require('../../assets/Minesweeper.png'),
                        link: 'https://cheffyjonny-minesweeper.netlify.app'
                    },
                    {
                        title: 'Javascript On Screen Calculator',
                        content: '-This is a basic calculator written by JavaScript.',
                        image: require('../../assets/JavascriptOnScreenCalculator.png'),
                        link: 'https://cheffyjonny-calculator.netlify.app'
                    },
                    {
                        title: 'Multi Brand Online Shop',
                        content: '-This is multi brand online shop.',
                        image: require('../../assets/MultiBrandOnlineshop.png'),
                        link: 'https://cheffyjonny-multistore-home.netlify.app'
                    },
                    {
                        title: 'Wikipedia Search Engine',
                        content: '-You can search something on here instead of Wikipedia :).',
                        image: require('../../assets/WikipediaSearchEngine.png'),
                        link: 'https://cheffyjonny-wikipedia.netlify.app'
                    },
                    {
                        title: 'Weather App With Weather Animation',
                        content: 'This is a weather application working with API.',
                        image: require('../../assets/WeatherAppWithWeatherAnimation.png'),
                        link: 'https://cheffyjonny-weatherapp.netlify.app'
                    }
                ]
            }
        }
    }
</script>

<style scoped></style>
