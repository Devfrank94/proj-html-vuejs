<script>

import {footMenu} from "../data/menus";
export default {
  name: "Footer",
  data(){
    return{
      footMenu,
    }
  }
}
</script>

<template>
  
  <footer>
    <div class="container">
      <div class="foot-cont d-flex flex-dir-col al-item-cent py-5">
        <img src="/img/logo_seo_2x.png" alt="Logo footer">
        <nav class="my-4">
          <ul class="d-flex al-item-cent">
            <li v-for="(link, index) in footMenu" :key="index">
              <a :href="link.href" :class="{'active' : link.isActive}">{{link.text}}</a>
            </li>
          </ul>
        </nav>
        <p>&copy; Copiright 2012 - 2020 | Avada Theme by <strong>ThemeFusion</strong> | All Rights Reserved | Powered by <strong>DevFrank</strong> </p>
        <div>
          Icone social
        </div>

      </div>
    </div>
  </footer>


</template>


<style lang="scss" scoped>
  @use '../scss/main.scss' as *;


  footer{

    .foot-cont{

      p{
        color: $gray;
        font-size: .7rem;
      }
    
      img{
      width: 130px;
      min-width: 80px;
      }

      ul{
      margin-top: 1rem;
      }


      a{
        display: inline-block;
        margin-right: 1.5rem;
        text-transform: capitalize;
        text-decoration: none;
        color: $gray;
        font-size: .8rem;
        font-weight: 600;
        &:hover,
        &.active{
          color: $bg-orange;
        }
      }

    }

  }


</style>