<script>
import { stringifyStyle } from '@vue/shared';

    export default{
            name: "DcCard",
            props: {
                img: String,
                prezzo: String,
                serie: String,
                tipo: String,
            },  
    }
</script>

<template>
        <div class="card">
            <img :src="img" alt="">
            <p>{{serie}}</p>
        </div>
        
</template>

<style lang="scss" scoped>
    
        .card{
            width: calc(100% / 6 - 2rem);
            height: 500px;
            background-color: red;
            margin: 2rem 1rem;
            p{  
                color: white;
                padding: 1rem 0rem;
            }
            img{
                width: 100%;
                height: 100%;
                object-fit: cover;
                object-position: top ;
            }
        }

    
</style>