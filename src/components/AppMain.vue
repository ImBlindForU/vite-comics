<script>
    import ListCards from './ListCards.vue';
    export default{
        name: "AppMain",
        components: {
            ListCards,
        }
    }
</script>

<template>
    <div class="container-fluid black">
        <div class="jumbo-container">
            <img src="../assets/img/jumbotron.jpg" alt="">
        </div>
        <ListCards  />
    </div>
</template>

<style lang="scss" scoped>
    .black{
        background-color: #1c1c1c;
    }
    .container-fluid{

        .jumbo-container{
            height: 800px;
            img{
                width: 100%;
                height: 100%;
                object-fit: cover;
                object-position: top;
            }
        }
    }

    
</style>