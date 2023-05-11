<script>

import {footMenu, socialIcon} from "../data/menus";
import BackToTop from './partials/BackToTop.vue';
export default {
  name: "Footer",
  components: {
    BackToTop
},
  data(){
    return{
      footMenu,
      socialIcon
    }
  }
}
</script>

<template>
  
  <footer>
    <div class="container">
      <div class="foot-cont d-flex flex-dir-col al-item-cent py-4">
        <img src="/img/logo_seo_2x.png" alt="Logo footer">
        <nav class="my-4">
          <ul class="d-flex al-item-cent">
            <li v-for="(link, index) in footMenu" :key="index">
              <a :href="link.href" :class="{'active' : link.isActive}">{{link.text}}</a>
            </li>
          </ul>
        </nav>
        <p class="mb-1">&copy; Copiright 2012 - 2020 | Avada Theme by <strong>ThemeFusion</strong> | All Rights Reserved | Powered by <strong>DevFrank</strong> </p>
        <ul class="d-flex al-item-cent">
          <li v-for="(icon, index) in socialIcon" :key="index">
            <a :href="icon.href"><i :class="icon.img"></i></a>
          </li>
        </ul>

      </div>
    </div>

    <!-- Back to Top Button -->
    <BackToTop/>

  </footer>


</template>


<style lang="scss" scoped>
  @use '../scss/main.scss' as *;


  footer{

    .foot-cont{

      ul{

        i{
          font-size: .9rem;
        }
        
      }

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