<script>
    export default{
        name: "AppHeader",
        data(){
            return{
                headerLinks: [
                    {
                        title:"CHARACTERS",
                        href: "/CHARACTERS",
                        active: false,
                    },
                    {
                        title:"COMICS",
                        href: "/COMICS",
                        active: false,

                    },
                    {
                        title:"MOVIES",
                        href: "/MOVIES",
                        active: false,

                    },
                    {
                        title:"TV",
                        href: "/TV",
                        active: false,

                    },
                    {
                        title:"GAMES",
                        href: "/GAMES",
                        active: false,

                    },
                    {
                        title:"COLLECTIBILES",
                        href: "/COLLECTIBILES",
                        active: false,

                    },
                    {
                        title:"VIDEO",
                        href: "/VIDEO",
                        active: false,

                    },
                    {
                        title:"FANS",
                        href: "/FANS",
                        active: false,

                    },
                    {
                        title:"NEWS",
                        href: "/NEWS",
                        active: false,

                    },
                    {
                        title:"SHOP",
                        href: "/SHOP",
                        active: false,

                    }
                ]
            }
        }
    }
</script>

<template>
    <div class="container-fluid white">
        <div class="container">
            <div class="logo-header">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <div class="menu">
                <ul>
                    <li v-for="(headerLink, index) in headerLinks" :key="index">
                        <a  :class="{ 'active': headerLink.active }" :href="headerLink.url">{{headerLink.title}}</a>
                    </li>
                    
                </ul>
                
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    .white{
        background-color: white;
    }
    .container-fluid{
        .logo-header{
            min-width: 70px;
            padding: 1rem;
        }
        .container{
        display: flex;
        justify-content: space-between;
        align-items: center;
        
        .menu{
            
            ul{
                list-style: none;
                display: flex;
                flex-direction: row;
                li{
                    margin: 0 1rem;
                    padding: 1rem;
                    line-height: 200px;

                    a{
                        position: relative;
                        display: inline-block;
                        text-decoration: none;
                        line-height:inherit;
                        color: black;
                        
                        &:hover{
                            color: #0282f9;
                            
                        }
                        &::after{
                            content: "";
                            width: 100%;
                            height: 0px;
                            position: absolute;
                            bottom: 0;
                            left: 0;
                            display: inline-block;
                            color: #0282f9;
                            background-color: #0282f9;
                            transition: height .3s ease;
                        }   
                        &:hover::after,
                        &.active::after {
                            height: 5px;
                        }                     
                    }  
                }
            }
        }
    }
    }
    
</style>