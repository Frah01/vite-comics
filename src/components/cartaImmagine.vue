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
            <h4>{{titolo}}</h4> 
        </div>
    </div>
</template>

<style lang="scss">
    .card{
        width: 130px;
       margin: 40px 0px;
       h4{
        color: white;
        word-break: break-all;
        font-size: 16px;
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