<script>
    export default{
        name: "AppFooter",
        data(){
            return{
                footerLinks:[
                    {
                        titleFooter:"DC COMICS",
                        subTitles:[
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
        }
        
    }
</script>

<template>
    <div class="container-fluid bk-img">
        <div class="container">
            <div class="top-footer">
                <div class="list-footer">
                    <ul>
                        <li v-for="(footerLink, index) in footerLinks" :key="index">
                            <h2>{{footerLink.titleFooter}}</h2>
                            <ul>
                                <li v-for="(subTitle, index) in footerLinks.subTitles" :key="index">
                                    {{subTitle.sub}}
                                </li>
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
    <div class="container-fluid grey">
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
        .container{
            height: 600px;
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
                    overflow: hidden;

                    img{
                        width: 100%;
                        height: 100%;
                        object-fit: cover;
                        object-position: centre;
                    }
                }
            }
        }
    }
    .grey{
        background-color: #303030;
    }
    .container-fluid{
   
        .bottom-footer{
            height: 200px;
            width: 70vw;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
        }
    }
</style>