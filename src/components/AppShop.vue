<script>
    export default{
        name: "AppShop",
        data(){
            return{
                shopLinks:[
                    {
                        imgText: "DIGITAL COMICS",
                        image: "../assets/img/buy-comics-digital-comics.png",
                    },
                    {
                        imgText: "DC MERCHANDISE",
                        image: "../assets/img/buy-comics-merchandise.png",
                    },
                    {
                        imgText: "SUBSCRIPTION",
                        image: "../assets/img/buy-comics-subscriptions.png",
                    },
                    {
                        imgText: "COMIC SHOP LOCATOR",
                        image: "../assets/img/buy-comics-shop-locator.png",
                    },
                    {
                        imgText: "DC POWER VISA",
                        image: "../assets/img/buy-dc-power-visa.png",
                    },
                ]
            }
        },
        methods: {
            getImagePath: function(imgPath){
                return new URL(imgPath, import.meta.url).href;
            }
        }
    }
</script>

<template>
     <div class="container-fluid blue">
        <div class="container">
            <ul>
                <li v-for="shopLink in shopLinks">
                    <span><img :src="getImagePath(shopLink.image)" alt=""></span>
                    <span><a href="">{{shopLink.imgText}}</a></span>
                </li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    .blue{
        background-color: #0282f9;
    }
    .container-fluid{
        .container{
            
            display: flex;
            align-items: center;
            ul{
                margin: 0 auto;
                list-style: none;
                display: flex;
                justify-content: space-between;
                li{
                    display: flex;
                    align-items: center;
                    padding: 3rem;
                    margin: 0 2rem;
                    span{
                        img{
                            
                            max-width: 70px;
                        }

                        a{
                            text-decoration: none;
                            color: white;
                        }
                        padding: 1rem;
                        color: white;
                    }
                }
            }
        }
    }
</style>