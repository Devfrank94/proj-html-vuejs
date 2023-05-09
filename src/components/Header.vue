<script>

import {mainMenu} from "../data/menus";
export default {
  name: "Header",
  data(){
    return{
      mainMenu
    }
  }
}
</script>

<template>

<div class="container test">
  <header class="d-flex j-cont-bet al-item-cent ">
    <div class="logo">
      <img src="/img/logo_seo_w_2x.png" alt="Logo Avada SEO">
    </div>
    <nav>
      <ul class="d-flex">
        <li v-for="(link, index) in mainMenu" :key="index">
          <a :href="link.href" :class="{'active' : link.isActive}">{{link.text}}</a>
        </li>
      </ul>
    </nav>

    <div class="fm-btn">get in touch now</div>
  </header>
</div>

</template>


<style lang="scss" scoped>

@use '../scss/main.scss' as *;


header{
  margin: 1rem 0;
  height: 70px;

  .logo{
    width: 160px;
    min-width: 100px;
  }

    ul{

      a{
        display: inline-block;
        margin: 0 .6rem;
        padding-top: 1rem;
        padding-bottom: 1rem;
        text-transform: capitalize;
        text-decoration: none;
        color: $white;
        font-size: 1rem;
        font-weight: 600;
        &:hover,
        &.active{
          color: $bg-orange;
        }
      }
    }

    
  }

</style>