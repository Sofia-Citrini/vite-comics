<template>
    <section class="py-5">
        <div class="container d-flex">
            <div class="d-flex align-items-center info">
                <div class="img-container info">
                    <img src="/imgs/buy-comics-digital-comics.png" class="img-fluid" alt="">
                </div>
                <div class="text"><a href="#">Digital Comics</a></div>
            </div>
            <div class="d-flex align-items-center info">
                <div class="img-container">
                    <img src="/imgs/buy-comics-merchandise.png" class="img-fluid" alt="">
                </div>
                <div class="text"><a href="#">DC merchandise</a></div>
            </div>
            <div class="d-flex align-items-center info">
                <div class="img-container">
                    <img src="/imgs/buy-comics-subscriptions.png" class="img-fluid" alt="">
                </div>
                <div class="text"><a href="#">Subscription</a></div>
            </div>
            <div class="d-flex align-items-center info">
                <div class="img-container">
                    <img src="/imgs/buy-comics-shop-locator.png" class="img-fluid" alt="">
                </div>
                <div class="text"><a href="#">comic shop locator</a></div>
            </div>
            <div class="d-flex align-items-center info">
                <div class="img-container">
                    <img src="/imgs/buy-dc-power-visa.svg" class="img-fluid" alt="">
                </div>
                <div class="text"><a href="#">dc power visa</a></div>
            </div>
        </div>
    </section>
   
</template>

<script>
    export default{
        data (){
        },
        methods: {
        } 
    }
</script>

<style scoped lang="scss">
    @use '../styles/partials/variables' as *;

    section {
        background-color: $color-primary;
    }

    .info{
        flex-basis: calc(100% / 5);
        justify-content: center;

        .img-container{
            width: 2rem;
        }

        .text{
            text-transform: uppercase;
            font-size: smaller;

            a{
                text-decoration: none;
                color: white;
                padding: .5rem;
            }
        }
    }
    

    
</style>