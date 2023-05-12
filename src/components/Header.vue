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

<div class="wrapper">

  <!-- ************JUMBOTRON********** -->
  <div id="jumbotr" class="jumbotron relative">
    <img src="/img/1-hero-image.png" alt="Jumbotron">
    <div class="fmcontainer absolute">
      <div class="leftblock">
        <h2>SEM campaigns made simple with avada</h2>
        <p class="my-4">Lorem ipsum dolor sit amet consectetur adipisicing elit. Vitae fugiat et, omnis itaque, perferendis perspiciatis minus cum sapiente</p>
        <span class="fm-btn btn-orange me-2 ">buy avada now</span>
        <span class="fm-btn btn-cyan">contact us</span>
      </div>
    </div>
  </div>

  <!-- ************/JUMBOTRON********** -->

  <!-- ************HEADER************* -->
  <div class="fmcontainer absolute">
    <header class="d-flex j-cont-bet al-item-cent ">
      <div class="logo">
        <img src="/img/logo_seo_w_2x.png" alt="Logo Avada SEO">
      </div>
      <nav>
        <ul class="d-flex al-item-cent">
          <li v-for="(link, index) in mainMenu" :key="index">
            <a :href="link.href" :class="{'active' : link.isActive}">{{link.text}}</a>
          </li>
        </ul>
      </nav>

      <div class="fm-btn btn-orange">get in touch now</div>
    </header>
  </div>
</div>
  <!-- ************/HEADER************* -->



</template>


<style lang='scss' scoped>

@use '../scss/main.scss' as *;

// ************HEADER*************

.wrapper{
    height: 100%;


  .fmcontainer{
    top: 0;
    left: 50%;
    translate: (-50% 0);
  }

}

header{
  margin: 1rem 0;
  height: 70px;

  .logo{
    width: 160px;
    min-width: 100px;
  }

    ul{
      margin-top: 1rem;

      li:nth-child(5){
        position: relative;
      }
      li:nth-child(6){
        margin-left: 2.5rem;
      }

      li:nth-child(5):after {
        content: 'apply';
        color: $bg-orange;
        position: absolute;
        top: 4px;
        left: 48px;
        border-radius: 5px;
        padding: 0 5px;
        border: 2px solid $bg-orange;
        text-align: center;
        text-transform: uppercase;
        font-weight: 600;
        font-size: .6rem;
        cursor: pointer;
      }
      
      li:nth-child(5):hover:after{
        color: white;
        background-color: $bg-orange;
      }


      a{
        display: inline-block;
        margin-right: 1.5rem;
        text-transform: capitalize;
        text-decoration: none;
        color: $white;
        font-size: .8rem;
        font-weight: 600;
        &:hover,
        &.active{
          color: $bg-orange;
        }
      }
      
  }
}
// ************/HEADER*************

// ************JUMBOTRON*************

.jumbotron{
  width: 100%;
  z-index: -1;

  .fmcontainer{
    top: 50%;
    left: 50%;
    translate: (-50% -50%);
    .leftblock{
    color: white;
    min-width: 20%;
    max-width: 50%;

    h2{
      text-transform: capitalize;
      font-size: 2.4rem;
      font-weight: 600;
    }

    p{
      font-size: .8rem;
      color: $bg-sect;
    }

    }
  }


}
// ************/JUMBOTRON*************

</style>