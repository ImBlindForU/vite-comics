<script>
    export default{
        name: "AppHeader",
        data(){
            return{
                headerLinks: [
                    {
                        title:"CHARACTERS",
                        href: "/CHARACTERS",
                    },
                    {
                        title:"COMICS",
                        href: "/COMICS",
                    },
                    {
                        title:"MOVIES",
                        href: "/MOVIES",
                    },
                    {
                        title:"TV",
                        href: "/TV",
                    },
                    {
                        title:"GAMES",
                        href: "/GAMES",
                    },
                    {
                        title:"COLLECTIBILES",
                        href: "/COLLECTIBILES",
                    },
                    {
                        title:"VIDEO",
                        href: "/VIDEO",
                    },
                    {
                        title:"FANS",
                        href: "/FANS",
                    },
                    {
                        title:"NEWS",
                        href: "/NEWS",
                    },
                    {
                        title:"SHOP",
                        href: "/SHOP",
                    }
                ]
            }
        }
    }
</script>

<template>
    <div class="container-fluid white">
        <div class="container-header">
            <div class="logo-header">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <div class="menu">
                <ul>
                    <li v-for="headerLink in headerLinks">
                        <a href="">{{headerLink.title}}</a>
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
        width: 100vw;
        .logo-header{
            padding: 1rem;
        }
        .container-header{
        
        width: 70vw;
        height: 10vh;
        margin: 0 auto;
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
                    line-height: calc(10vh - 2rem);
                    
                    a{
                        text-decoration: none;
                        color: black;
                        &:hover{                 
                            color: #0282f9;
                        }
                    }
                    &:hover{
                        box-shadow: 0px -10px #0282f9 inset;
                        }
                    
                }
            }
        }
    }
    }
    
</style>