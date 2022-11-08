<script>
    export default{
        name: "AppFooter",
        footerLinks:[
                    {
                        titleFooter:"DC COMICS",
                        subTitle:[
                            {
                                sub:"Characters"
                            },
                            {
                                sub:"Comics"
                            },
                            {
                                sub:"Movies"
                            },
                            {
                                sub:"TV"
                            },
                            {
                                sub:"Games"
                            },
                            {
                                sub:"Videos"
                            },
                            {
                                sub:"News"
                            },
                        ]
                    },
                    {
                        titleFooter:"SHOP",
                        subTitle:[
                            {
                                sub:"Shop DC"
                            },
                            {
                                sub:"Shop DC Collectibles"
                            },
                            
                        ]
                    },
                    {
                        titleFooter:"DC",
                        subTitle:[
                            {
                                sub:"Terms Of Use"
                            },
                            {
                                sub:"Privacy policy(New)"
                            },
                            {
                                sub:"Ad Choices"
                            },
                            {
                                sub:"Advertising"
                            },
                            {
                                sub:"Jobs"
                            },
                            {
                                sub:"Subscriptions"
                            },
                            {
                                sub:"Talent Workshop"
                            },
                            {
                                sub:"CPSC Certificates"
                            },
                            {
                                sub:"Ratiings"
                            },
                            {
                                sub:"Shop Help"
                            },
                            {
                                sub:"Contacts Us"
                            },
                        ]
                    },
                    {
                        titleFooter:"SITES",
                        subTitle:[
                            {
                                sub:"DC"
                            },
                            {
                                sub:"MAD Megazine"
                            },
                            {
                                sub:"DC Kids"
                            },
                            {
                                sub:"DC Universe"
                            },
                            {
                                sub:"DC Power Visa"
                            },
                            
                        ]
                    },
                    
                ]
    }
</script>

<template>
    <div class="container-fluid bk-img">
        <div class="container-main">
            <div class="top-footer">
                <div class="list-footer">
                    <ul>
                        <li v-for="footerLink in footerLinks">
                            <h2>{{footerLink.titleFooter}}</h2>
                            <ul>
                                <li>{{footerLink.subTitle.sub}}</li>
                            </ul>
                        </li>
                    </ul>
                </div>
                <div class="img-footer">
                    <img src="../assets/img/dc-logo-bg.png" alt="">
                </div>
            </div>
            
        </div>
        
    </div>
    <div class="container-fluid-two grey">
        <div class="bottom-footer">
                <div class="btn">
                    <a href="">SING-UP NOW!</a>
                </div>
                <div class="social">

                </div>
        </div>
    </div>
       
</template>

<style lang="scss" scoped>
    .bk-img{
        background-image: url(../assets/img/footer-bg.jpg);
        background-position: center;
        background-size: cover;
    }
    .container-fluid{
        width: 100vw;
        .container-main{
            width: 70vw;
            height: 50vh;
            margin: 0 auto;
            .top-footer{
                display: flex;
                justify-content: space-between;
                
                .list-footer{
                    
                    ul{
                        list-style: none;
                        h2{
                            font-size: 2rem;
                        }
                        li{
                            color: white;
                            ul{
                                li{
                                    color: red;
                                }
                            }
                        }
                    }
                }
                .img-footer{
                    
                    img{
                        width: 40vw;
                       
                    }
                }
            }
        }
    }
    .grey{
        background-color: #303030;
    }
    .container-fluid-two{
        width: 100vw;
        .bottom-footer{
            height: 10vh;
            width: 70vw;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
        }
    }
</style>