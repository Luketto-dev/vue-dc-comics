<template>
  <div id="app">
    <TheHeader></TheHeader>
    <section class="content py-5">
      <div class="container">
        <div class="content-text">-->Content goes here</div>
      </div>
    </section>
    <TheBanner></TheBanner>
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue'
import TheBanner from './components/TheBanner.vue'



export default {
  name: 'App',
  components: {
    TheHeader,
    TheBanner,
  }
}
</script>

<style lang="scss">
@import "assets/scss/main.scss";

</style>
