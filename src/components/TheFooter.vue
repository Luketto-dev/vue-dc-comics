<template>
    <footer>
        <div class="container">
            <div class="row justify-content-between">
                <div class="col-4 py-4">
                    <div class="row">
                        <div class="col-4">
                            <div class="links-title text-white">
                                <h5>DC COMICS</h5>
                            </div>
                            <ul class="list-unstyled footer-list">
                                <li v-for="link in dcComicsLinks" :key="link">
                                    {{link}}
                                </li>
                            </ul>                
                        </div>
                        <div class="col-4">
                            <div class="links-title text-white">
                                <h5>DC</h5>
                            </div>
                            <ul class="list-unstyled footer-list">
                                <li v-for="link in dcLinks" :key="link">
                                    {{link}}
                                </li>
                            </ul>                
                        </div>
                        <div class="col-4">
                            <div class="links-title text-white">
                                <h5>Sites</h5>
                            </div>
                            <ul class="list-unstyled footer-list">
                                <li v-for="link in sitesLinks" :key="link">
                                    {{link}}
                                </li>
                            </ul>                
                        </div>
                    </div>
                </div>
                <div class="col-5 overflow-hidden">
                    <div class="dc-logo position-relative">
                        <img src="/img/dc-logo-bg.png" alt="">
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default{
    data() {
        return{
            dcComicsLinks:[
                "Characters",
                "comics",
                "Movies",
                "TV",
                "Games",
                "Videos",
                "News",            
                ],
                dcLinks:[
                "Terms Of Use",
                "Privacy Policy",
                "Ad Choices",
                "Adversting",
                "Jobs",
                "Subscriptions",
                "Talent Worshops", 
                "CPSC Certificates",
                "Ratings",
                "Shop Help",
                "Contact Us"           
                ],
                sitesLinks:[
                    "DC",
                    "Mad Magazine",
                    "DC Kids",
                    "DC Universe",
                    "DC Power Visa"
                ]

        }
    }
}
</script>


<style lang="scss">
footer{
    background-image: url('/public/img/footer-bg.jpg');
    background-size: cover ;
    background-position: center;
    


    & .links-title h5{
        font-size: 1rem;
        font-weight: bold;
    }

    & .footer-list{
        color: #878878;
        font-size: .7rem;
    }

    & .dc-logo img{
        width: 90%;
        position: absolute;
        top: -100px;
        
    }


}
</style>