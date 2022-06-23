<template>
    <div class="my-card">
        <img :src="urlImg" alt="">
        <div class="my-card-title">
            <h6 class="text-white pt-3">{{cardTitle}}</h6>
        </div>

    </div>
</template>


<script>


export default{
    props:{
        urlImg: String,
        cardTitle : String,
        comicPrice: String,
        comicType: String,
    },
    data(){
        return{

        }
    }
}
</script>


<style lang="scss" scoped>
.my-card{
    aspect-ratio: 1/1;

    & img{
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: top;
    }
}
</style>