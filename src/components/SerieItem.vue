<template>
    <div class="my-card">
        <div>
            <img :src="serie.thumb" alt="" class="img-fluid">
        </div>
        <div>{{serie.series}}</div>
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

</style>