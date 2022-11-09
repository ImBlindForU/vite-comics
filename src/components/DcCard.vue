<script>
import { stringifyStyle } from '@vue/shared';

    export default{
        components:{
            name: "DcCard",
            props: {
                img: String,
                prezzo: String,
                serie: String,
                tipo: String,
            },
        }
    }
</script>

<template>
        <div class="card">
            <img :src="thumb" alt="">
        </div>
        
</template>

<style lang="scss" scoped>
    
        .card{
            width: calc(100% / 6 - 2rem);
            height: 300px;
            background-color: red;
            margin: 1rem;
            img{
                width: 100%;
                height: 100%;
                object-fit: cover;
                object-position: top ;
            }
        }

    
</style>