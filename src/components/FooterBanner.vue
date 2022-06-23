<template>
    <div class="banner-social py-4">
        <div class="container">
            <div class="d-flex justify-content-between">
                <button class="btn btn-secondary">SING-UP NOW</button>
                <div class="follow-us d-flex align-items-center">
                    <h6 class="">FOLLOW US</h6>
                    <a class="p-2" v-for="social in socials" :key="social" href="">
                        <img class="w-100" :src="'./img/' + social" alt="">
                    </a>
                </div>
            </div>
        </div>
    </div>
</template>


<script>
export default{
    data(){
        return{
            socials:[
                "footer-facebook.png",
                "footer-twitter.png",
                "footer-youtube.png",
                "footer-pinterest.png",
                "footer-periscope.png"
            ]
        }
    }
}
</script>


<style lang="scss" scoped>
.banner-social{
    background-color: #303030;

    & .btn-secondary{
        border-radius: 0;
        border: 2px solid #0282F9;
        background-color: inherit;
        padding-top: .7rem;
        padding-bottom: .7rem;
    }

    & h6{
        color: #0282F9;
        font-weight: bold;
        padding-right: 1rem;
        margin: 0;
    }
}
</style>