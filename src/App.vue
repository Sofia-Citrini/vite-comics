

<template>
  <TheHeader></TheHeader>

  <main>
    <div class="content">Content</div>
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

  export default{
    components: { TheHeader, TheFooter, BannerFooter, BannerInfo },
    data() {
      return{}
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
