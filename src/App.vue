<template>
  <div id="app">
    <Header />
    <Main />
    <Footer />
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'
export default {
  name: 'App',
  components: {
    // HelloWorld,
    Header,
    Main,
    Footer,
  }
}
</script>

<style lang="scss">
@import "./assets/scss/style.scss"
</style>