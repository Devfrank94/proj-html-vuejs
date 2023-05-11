<script>
import { store } from "../../data/store.js";
export default {
  name:"BackToTop",
  data(){
    return{
      store
    }
  },
  methods:{
    checkScroll(){
      window.addEventListener("scroll", () =>{
        window.scrollY > 20 ? store.showBackUp = true : store.showBackUp = false;
      })
    }
  },
  mounted(){
    this.checkScroll()
  }
}
</script>

<template>
  <a href="#jumbotr" :class="{'show' : store.showBackUp}"><i class="fa-solid fa-chevron-up fa-sm" style="color: white;"></i></a>
</template>

<style lang="scss" scoped>
@use '../../scss/main.scss' as *;


  a{
    position: fixed;
    bottom: 0px;
    right: 70px;
    opacity: 0;
    background-color: $gray;
    border-radius: 5px 5px 0 0;
    width: 50px;
    height: 40px;
    display: flex;
    justify-content: center;
    align-items: center;
    transition: all .5s;

    &.show{
      bottom: 0;
      opacity: 1;
    }
  }
</style>