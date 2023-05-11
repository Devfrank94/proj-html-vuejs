
<script>

import Header from "./components/Header.vue"
import Main from "./components/Main.vue"
import Footer from "./components/Footer.vue"

export default {
  name:'App',
  components:{
    Header,
    Main,
    Footer
  }
}
</script>
<template>
  <html>
    
  <Header />

  <Main />

  <Footer />

  </html>
</template>


<style lang="scss">

  @use './scss/main.scss' as *;

  html {
  scroll-behavior: smooth;
  
  }

</style>