<template>
    <header>
        <div class="container">
            <nav class="d-flex justify-content-between py-3">
                <div class="logo">
                    <img src="../../public/img/dc-logo.png" alt="">
                </div>
                <ul class="my-navbar d-flex align-items-center list-unstyled">
                    <li v-for="(link, i) in navbarLinks" :key="i" class="my-navbar-item">
                        <a class="p-3 text-uppercase" :href="link.href">{{link.nome}}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default{
    data() {
        return{
            navbarLinks:[
                {
                    nome: "characters",
                    href: "#"
                },
                {
                    nome: "comics",
                    href: "#"
                },
                {
                    nome: "movies",
                    href: "#"
                },
                {
                    nome: "tv",
                    href: "#"
                },
                {
                    nome: "games",
                    href: "#"
                },
                {
                    nome: "collectibles",
                    href: "#"
                },
                {
                    nome: "videos",
                    href: "#"
                },
                {
                    nome: "fans",
                    href: "#"
                },
                {
                    nome: "news",
                    href: "#"
                },
                {
                    nome: "shop",
                    href: "#"
                },
            ]
        }
    }
}
</script>


<style lang="scss">
    .logo{
        width: 80px;

        & img{
            width: 100%;
        }
    }

    .my-navbar{
        font-size: .7rem;
        font-weight: bold;
        margin: 0;


        & .my-navbar-item a{
            color: black;
            text-decoration: none;
            display: block;
            border-bottom: 2px solid transparent;

            &:hover{
                color:#0282F9;
                border-bottom: 2px solid #0282F9;
            }

            
        }
    }
</style>