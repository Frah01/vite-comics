<script>

export default {
    props: {
        image: String,
        titolo: String,
    }
}
</script>
<template lang="">
    <div>
        <div class="card" >
            <div class="card-img" >
                <img :src="image" alt="">
            </div>
            <p>{{titolo}}</p> 
        </div>
    </div>
</template>

<style lang="scss">
    .card{
        width: 130px;
        margin: 20px 5px;
        text-transform: uppercase;
       p{
        color: white;
        word-break: break-all;
        font-size: 10px;
        margin-top: 10px
       }
    }
    

    .card-img{
        height: 130px;
        overflow: hidden;

        img{
            max-width: 100%;
        }
    }
</style>