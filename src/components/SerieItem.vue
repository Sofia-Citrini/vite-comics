<template>
    <div class="my-card">
        <div class="ratio ratio-1x1">
            <img :src="serie.thumb" alt="" class="img-fluid">
        </div>
        <div class="text-card">{{serie.series}}</div>
    </div>
</template>

<script>
    export default{
        props: {
            serie: Object
        }
    }

</script>

<style scoped lang="scss">
   .img-fluid{
    object-fit: cover;
    object-position: top;
   }

   .text-card{
    color: white;
    font-size: x-small;
    text-transform: uppercase;
    padding: .5rem 0;
   }
</style>