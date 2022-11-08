<script>
    export default{
        name: "AppMain"
    }
</script>

<template>
    <div class="container-fluid black">
        <div class="container-main">
            <h1> --arrow Content go here-- </h1>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    .black{
        background-color: black;
    }
    .container-fluid{
        width: 100vw;
        .container-main{
            width: 70vw;
            height: 10vh;
            margin: 0 auto;

            display: flex;
            justify-content: flex-start;
            align-items: center;
            h1{
            color: white;
            }
        }
    }

    
</style>