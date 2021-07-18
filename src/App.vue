<template>
    <div id="app">
        <Header />
        <Banner />
        <Headline />
        <NewsRead />
        <Crew />
        <Footer />
        <!-- footer -->
        <div id="popup-backdrop"></div>
    </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Banner from '@/components/Banner.vue'
import Headline from '@/components/Headline.vue'
import NewsRead from '@/components/NewsRead.vue'
import Crew from '@/components/Crew.vue'
import Footer from '@/components/Footer.vue'

export default {
    name: 'App',
    components: {
        Header,
        Banner,
        Headline,
        NewsRead,
        Crew,
        Footer,
    }
}
</script>