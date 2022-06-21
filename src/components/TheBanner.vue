<template>
    <div class="banner">
        <div class="container">
            <ul class="banner-list d-flex align-items-center list-unstyled m-0">
                <li class="banner-item text-uppercase" v-for="(bunnerLink, i) in bunnerLinks" :key="i">
                    <a href="">
                        <img :src="'../../public/img/' + bunnerLink.img" alt="">
                        <div>{{bunnerLink.nome}}</div>
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default{
    data() {
        return{
            bunnerLinks: [
                {
                    img : "buy-comics-digital-comics.png",
                    nome: "digital comics"
                },
                {
                    img : "buy-comics-merchandise.png",
                    nome: "dc merchandise"
                },
                {
                    img : "buy-comics-subscriptions.png",
                    nome: "subscription"
                },
                {
                    img : "buy-comics-shop-locator.png",
                    nome: "comic shop locator"
                },
                {
                    img : "buy-dc-power-visa",
                    nome: "digital comics"
                },
            ]
        }
    }
}
</script>


<style lang="scss">
.banner{
    background-color: #0282F9;

    & .banner-item{
    flex-basis: calc(100% / 5);
    flex-shrink: 0;

    & a{
        padding: 2rem;
        color: white;
        text-decoration: none;
        font-size: .8rem;
        display: block;
    }
}
}

</style>