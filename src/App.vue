

<template>
  <TheHeader></TheHeader>

  <main>
    <div class="content">Content</div>
  </main>

  <TheFooter></TheFooter>
  <BannerFooter></BannerFooter>
</template>

<script>
  import TheHeader from './components/TheHeader.vue';
  import TheFooter from './components/TheFooter.vue';
import BannerFooter from './components/BannerFooter.vue';

  export default{
    data() {
    },
    methods: {},
    components: { TheHeader, TheFooter, BannerFooter }
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
