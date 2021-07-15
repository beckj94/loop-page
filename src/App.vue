<template>
    <div id="app">
        <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
        <!-- header -->
        <Header />
        <!-- banner -->
        <Banner />
        <!-- headline -->
        <Headline />
        <!-- news read -->
        <NewsRead />
        <!-- crew -->
        <Crew />
        <!-- footer -->
    </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Banner from '@/components/Banner.vue'
import Headline from '@/components/Headline.vue'
import NewsRead from '@/components/NewsRead.vue'
import Crew from '@/components/Crew.vue'

export default {
    name: 'App',
    components: {
        Header,
        Banner,
        Headline,
        NewsRead,
        Crew,
    }
}
</script>