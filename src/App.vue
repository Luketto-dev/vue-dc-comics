<template>
  <div id="app">
    <TheHeader></TheHeader>
    <main class="bg-dark">
      <div class="jumbotron">
        <img src="../public/img/jumbotron.jpg" alt="">
      </div>
      <div class="container">
        <ComicsList></ComicsList>
      </div>
    </main>
    <TheBanner></TheBanner>
    <TheFooter></TheFooter>
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue'
import TheBanner from './components/TheBanner.vue'
import TheFooter from './components/TheFooter.vue'
import ComicsList from './components/ComicsList.vue'



export default {
  name: 'App',
  components: {
    TheHeader,
    TheBanner,
    TheFooter,
    ComicsList,
  }
}
</script>

<style lang="scss">
@import "assets/scss/main.scss";

</style>
