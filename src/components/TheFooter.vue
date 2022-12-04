<template>
    <footer>
        <div class="container">
            <div class="row">
                <div class="col-4 py-3">
                    <div class="row">
                        <div class="col-4 d-flex flex-column justify-content-between">
                            <div>
                                <h6>DC COMICS</h6>
                                <ul>
                                    <li><a href="#">Charachters</a></li>
                                    <li><a href="#">Comics</a></li>
                                    <li><a href="#">Movies</a></li>
                                    <li><a href="#">Tv</a></li>
                                    <li><a href="#">Games</a></li>
                                    <li><a href="#">Videos</a></li>
                                    <li><a href="#">News</a></li>
                                </ul>
                            </div>

                            <div>
                                <h6>SHOP</h6>
                                <ul>
                                    <li><a href="#">Shop DC</a></li>
                                    <li><a href="#">Shop DC Collection</a></li>
                                </ul>
                            </div>
                        </div>
                        <div class="col-4">
                            <h6>DC</h6>
                            <ul>
                                <li><a href="#">Terms Of Use</a></li>
                                <li><a href="#">Privacy policy (new)</a></li>
                                <li><a href="#">Ad Choices</a></li>
                                <li><a href="#">Advertising</a></li>
                                <li><a href="#">Jobs</a></li>
                                <li><a href="#">Subscriptions</a></li>
                                <li><a href="#">Talent Workshop</a></li>
                                <li><a href="#">CPSC Certifications</a></li>
                                <li><a href="#">Rating</a></li>
                                <li><a href="#">Shop Help</a></li>
                                <li><a href="#">Contact Us</a></li>
                            </ul>
                        </div>
                        <div class="col-4">
                            <h6>SITIES</h6>
                            <ul>
                                <li><a href="#">DC</a></li>
                                <li><a href="#">MAD Magazine</a></li>
                                <li><a href="#">DC Kids</a></li>
                                <li><a href="#">DC Universe</a></li>
                                <li><a href="#">DC Power Visa</a></li>
                            </ul>
                        </div>
                    </div>
                </div>

                <div class="col-8 img-container">
                    <img src="/imgs/dc-logo-bg.png" class="img-fluid" alt="">
                </div>
            </div>
        </div>
    </footer>
    
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

    footer{
        background-image: url("/imgs/footer-bg.jpg");
        // height: 400px ;
    }

    h6{
        font-weight: bold;
        color: white;
    }

    ul{
        list-style: none;
        padding-left: 0;

        a {
            text-decoration: none;
            color: $text-color-footer;
            font-size: small;
        }
    }

    .img-container {
        height: 400px;
        display: flex;
        justify-content: center;
        align-items: center;
        overflow: hidden;
    }
    
</style>