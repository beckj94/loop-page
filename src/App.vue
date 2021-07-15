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
        <!-- footer -->
    </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Banner from '@/components/Banner.vue'
import Headline from '@/components/Headline.vue'
import NewsRead from '@/components/NewsRead.vue'

export default {
    name: 'App',
    components: {
        Header,
        Banner,
        Headline,
        NewsRead,
    }
}
</script>