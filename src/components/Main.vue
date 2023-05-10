<script>
export default {
  name:'Main',
  data(){
    return {
    
    }
  },
}

</script>
<template>

  <!-- *********2. Main********** -->
  <main>

  <!-- *****2.1 - Section 1 Meet New Agency***** -->

  <section class="Sect1">
    <div class="container">
      <div class="title-cont mt-2 d-flex flex-dir-col al-item-cent">
        <h3 class="mt-5 mb-4">meet the new agency SEO template<br>from the avada team</h3>
        <p class="mb-5">Lorem ipsum dolor sit amet consectetur adipisicing elit. <br> Dolor, nam voluptas dolorum placeat libero itaque?</p>
      </div>

        <!-- ****CARDS**** -->
      <div class="row row-cols-3">
        <div class="cont-card">
          <div class="fmcard py-5 px-5 bg-white">
            <i class="fa-solid fa-road fa-xl" style="color: #ffa737;"></i>
            <div class="title-cont d-flex flex-dir-col al-item-cent">
              <h4 class="mt-3 mb-2">establish goals</h4>
              <p class="mb-2">Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolor, nam voluptas dolorum placeat libero</p>
            </div>
          </div>
        </div>
        <div class="cont-card">
          <div class="fmcard py-5 px-5 bg-white">
            <i class="fa-solid fa-video fa-xl" style="color: #ffa737;"></i>
            <div class="title-cont d-flex flex-dir-col al-item-cent">
              <h4 class="mt-3 mb-2">work with a team</h4>
              <p class="mb-2">Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolor, nam voluptas dolorum placeat libero</p>
            </div>
          </div>
        </div>
        <div class="cont-card">
          <div class="fmcard py-5 px-5 bg-white">
            <i class="fa-solid fa-droplet fa-xl" style="color: #ffa737;"></i>
            <div class="title-cont d-flex flex-dir-col al-item-cent">
              <h4 class="mt-3 mb-2">get results</h4>
              <p class="mb-2">Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolor, nam voluptas dolorum placeat libero</p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- ****/CARDS**** -->

    <!-- ****IMG SEO DESK**** -->
    <div class="container-fluid w-75">
      <img src="/img/agency-seo-desk-front-1200x570.jpg" alt="Seo Desk">
    </div>
  </section>


<!-- *****2.2 - Section 2 See Our Top Notch***** -->

<section class="Sect2">
    <div class="container">
      <div class="title-cont d-flex flex-dir-col al-item-cent">
        <h3 class="mt-5 mb-4">see our top notch services</h3>
        <p class="mb-5">Lorem ipsum dolor sit amet consectetur adipisicing elit. <br> Dolor, nam voluptas</p>
      </div>

        <!-- ****CARDS BLUE**** -->
      <div class="row row-cols-4">
        <div class="cont-card">
          <div class="fmcard py-5 px-5">
            <i class="fa-brands fa-google fa-xl" style="color: #ffa737;"></i>
            <div class="title-cont d-flex flex-dir-col al-item-cent">
              <h4 class="mt-3 mb-2">google SEO</h4>
              <p class="mb-3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolor, nam voluptas dolorum placeat libero</p>
              <span>read more</span>
            </div>
          </div>
        </div>
        <div class="cont-card">
          <div class="fmcard py-5 px-5">
            <i class="fa-solid fa-gear fa-xl" style="color: #ffa737;"></i>
            <div class="title-cont d-flex flex-dir-col al-item-cent">
              <h4 class="mt-3 mb-2">brand strategy</h4>
              <p class="mb-3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolor, nam voluptas dolorum placeat libero</p>
              <span>read more</span>
            </div>
          </div>
        </div>
        <div class="cont-card">
          <div class="fmcard py-5 px-5">
            <i class="fa-solid fa-building fa-xl" style="color: #ffa737;"></i>
            <div class="title-cont d-flex flex-dir-col al-item-cent">
              <h4 class="mt-3 mb-2">local SEO</h4>
              <p class="mb-3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolor, nam voluptas dolorum placeat libero</p>
              <span>read more</span>
            </div>
          </div>
        </div>
        <div class="cont-card">
          <div class="fmcard py-5 px-5">
            <i class="fa-solid fa-chart-column fa-xl" style="color: #ffa737;"></i>
            <div class="title-cont d-flex flex-dir-col al-item-cent">
              <h4 class="mt-3 mb-2">SEO analysis</h4>
              <p class="mb-3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolor, nam voluptas dolorum placeat libero</p>
              <span>read more</span>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- ****/CARDS BLUE**** -->
  </section>











  </main>

  
</template>


<style lang="scss" scoped>

  @use '../scss/main.scss' as *;

  // 2. Main
  // *******2.1 - Section 1 Meet New Agency********
  section:nth-child(odd){
    background-color: $bg-sect;  
  }

  .title-cont{

    h3{
    font-size: 1.3rem;
    font-weight: 700;
    }

    h4{
    font-size: 1rem;
    font-weight: 800;
    }

    p{
    font-size: .8rem;
    color: $gray;
    }
 
  }

  .fmcard{
    border-radius: 5px;

    p{
    font-size: .7rem;
    }
  }

  // *******/2.1 - Section 1 Meet New Agency********

  // ******2.2 - Section 2 See Our Top Notch******

.Sect2{
  padding-bottom: 100px;
  background-color: $bg-blue;
  background-image: url('/img/pattern_background.png');
  background-size: contain;

  h3{
    color: $bg-sect;
  }

  p{
    color: $bg-rocard;
  }

  .fmcard{
    background-color: $blue;

    h4{
      color: $bg-sect;
    }

    span{
      text-transform: capitalize;
      position: relative;
      color: $bg-orange;
      cursor: pointer;
      &:after {
        content: '>';
        position: absolute;
        color: $bg-orange;
        top: 0;
        right: -14px;
        font-size: 1.2rem;
      }
    }

  }


}
// ******/2.2 - Section 2 See Our Top Notch******

// ******2.3 - Section 3 Our Work******









// ******/2.3 - Section 3 Our Work*****





  
</style>