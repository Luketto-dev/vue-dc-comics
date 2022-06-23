<template>
  <div id="app">
    <TheHeader></TheHeader>
    <main class="bg-dark">
      <div class="jumbotron position-relative">
        <img src="../public/img/jumbotron.jpg" alt="">
      </div>
      <div class="container position-relative">
        <div class="label-current-series">CURRENT SERIES</div>
        <ComicsList></ComicsList>
        <div class="text-center pb-2">
          <button class="btn btn-primary">LOAD MORE</button>
        </div>
      </div>
    </main>
    <TheBanner></TheBanner>
    <TheFooter></TheFooter>
    <FooterBanner></FooterBanner>
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue'
import TheBanner from './components/TheBanner.vue'
import TheFooter from './components/TheFooter.vue'
import ComicsList from './components/ComicsList.vue'
import FooterBanner from './components/FooterBanner.vue'



export default {
  name: 'App',
  components: {
    TheHeader,
    TheBanner,
    TheFooter,
    ComicsList,
    FooterBanner
  }
}
</script>

<style lang="scss">
@import "./assets/scss/main.scss";

.btn-primary{
  border-radius: 0;
  padding: .3rem 2.5rem;
  background-color: #0282F9;
  font-size: .8rem;
}


</style>
