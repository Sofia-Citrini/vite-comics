<template>
  <TheHeader :menu="menuList"></TheHeader>

  <main>
    <SeriesList></SeriesList>
  </main>

  <BannerInfo></BannerInfo>

  <TheFooter></TheFooter>
  
  <BannerFooter></BannerFooter>
</template>

<script>
  import TheHeader from './components/TheHeader.vue';
  import TheFooter from './components/TheFooter.vue';
  import BannerFooter from './components/BannerFooter.vue';
  import BannerInfo from './components/BannerInfo.vue';
  import SeriesList from './components/SeriesList.vue'

  export default{
    components: { TheHeader, TheFooter, BannerFooter, BannerInfo, SeriesList },
    data() {
      return{
        menuList:[
          "charachters",
          "comics",
          "movies",
          "tv",
          "games",
          "collectibles",
          "videos",
          "fans",
          "news",
          "shop"
        ]
      }
    },
    methods: {},
  }
</script>

<style lang="scss">
  @use "./styles/general.scss";

  .content{
    height: 100px;
    color: white;
    background-color: black;
  }
</style>
