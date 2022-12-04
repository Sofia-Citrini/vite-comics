<template>
    <section class="banner py-4">
        <div class="container d-flex justify-content-between">
            <div>
                <button>sign up now!</button>
            </div>

            <div class="social">
                <div class="text">follow us</div>
                <img src="/imgs/footer-facebook.png" class="icon-social" alt="">
                <img src="/imgs/footer-twitter.png" class="icon-social" alt="">
                <img src="/imgs/footer-youtube.png" class="icon-social" alt="">
                <img src="/imgs/footer-pinterest.png" class="icon-social" alt="">
                <img src="/imgs/footer-periscope.png" class="icon-social" alt="">
            </div>
        </div>
    </section>
    
</template>

<script>
    export default{
        data (){
            return
        },
        methods: {
        }
            
    }
</script>

<style scoped lang="scss">
    @use '../styles/partials/variables' as *;

    .banner{
        background-color: $color-secondary;
    }

    button{
        border: 2px solid $color-primary;
        background-color: transparent;
        text-transform: uppercase;
        color: white;
        padding: .5rem;
    }

    .social{
        display: flex;
        align-items: center;

        .text{
            color: $color-primary;
            text-transform: uppercase;
            padding: 0 .5rem;
        }

        img{
            height: 1.5rem;
            margin: 0 .5rem;
        }
    }

</style>