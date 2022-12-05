<template>
    <footer>
        <div class="container">
            <div class="row">
                <div class="col-4 py-3">
                    <div class="row">
                        <div class="col col-md-4 d-flex flex-column justify-content-between">
                            <div>
                                <h6>DC COMICS</h6>
                                <ul>
                                    <li v-for="link in comicsLinks"><a :href="link.url">{{link.text}}</a></li>
                                </ul>
                            </div>

                            <div>
                                <h6>SHOP</h6>
                                <ul>
                                    <li v-for="link in shopLinks"><a :href="link.url">{{link.text}}</a></li>
                                </ul>
                            </div>
                        </div>
                        <div class="col col-md-4">
                            <h6>DC</h6>
                            <ul>
                                <li v-for="link in dcLinks"><a :href="link.url">{{link.text}}</a></li>
                            </ul>
                        </div>
                        <div class="col col-md-4">
                            <h6>SITIES</h6>
                            <ul>
                                <li v-for="link in sitiesLinks"><a :href="link.url">{{link.text}}</a></li>
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
    import { footerComicsLinks, footerShopLinks, footerDcLinks, footerSitiesLinks} from "../composables/footerLinks";

    export default{
       data (){
        return {
            comicsLinks: footerComicsLinks,
            shopLinks: footerShopLinks,
            dcLinks: footerDcLinks,
            sitiesLinks: footerSitiesLinks
        }
       }
    }
</script>

<style scoped lang="scss">
    @use '../styles/partials/variables' as *;

    footer{
        background-image: url("/imgs/footer-bg.jpg");
        background-size: cover;
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