<template>
    <header class="py-3">
        <div class="container d-flex justify-content-between">
            <div class="img-container">
                <img src="/imgs/dc-logo.png" alt="" class="img-fluid">
            </div>

            <nav class="navbar navbar-expand-lg">
                <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
                    <div class="navbar-nav">
                        <a class="nav-item nav-link" href="#" v-for="element in menuList">{{element}}</a>
                        <!-- <a class="nav-item nav-link" href="#">characters</a>
                        <a class="nav-item nav-link" href="#">comics</a>
                        <a class="nav-item nav-link" href="#">movies</a>
                        <a class="nav-item nav-link" href="#">tv</a>
                        <a class="nav-item nav-link" href="#">games</a>
                        <a class="nav-item nav-link" href="#">collectibles</a>
                        <a class="nav-item nav-link" href="#">videos</a>
                        <a class="nav-item nav-link" href="#">fans</a>
                        <a class="nav-item nav-link" href="#">news</a>
                        <a class="nav-item nav-link" href="#">shop</a> -->
                    </div>
                </div>
            </nav>
        </div>
    </header>
</template>

<script>
    export default{
        data (){
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
        methods: {
            
        }
    }
</script>

<style scoped lang="scss">
    @use '../styles/partials/variables' as *;
    .img-container {
        width: 3rem;
    }
    .nav-link{
        color: $text-color;
        text-transform: uppercase;
        font-size: .8rem;

        &:hover{
            color: $color-primary;
        }
    }
</style>