<script>
    export default{
        name: "AppHeader"
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
                    <li><a href=""></a>HOME</li>
                    <li><a href=""></a>HOME</li>
                    <li><a href=""></a>HOME</li>
                    <li><a href=""></a>HOME</li>
                    <li><a href=""></a>HOME</li>
                    <li><a href=""></a>HOME</li>
                    <li><a href=""></a>HOME</li>
                    <li><a href=""></a>HOME</li>
                    <li><a href=""></a>HOME</li>
                    <li><a href=""></a>HOME</li>

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
                    line-height: calc(10vh - 2rem);
                    padding: 1rem;
                    &:hover{
                        
                        color: #0282f9;
                        box-shadow: 0px -10px #0282f9 inset;
                        
                    }
                }
            }
        }
    }
    }
    
</style>