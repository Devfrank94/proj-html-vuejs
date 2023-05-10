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
      <div class="title-cont d-flex flex-dir-col al-item-cent">
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

  </section>
















  </main>

  
</template>


<style lang="scss" scoped>

  @use '../scss/main.scss' as *;

  // 2. Main
  // - 2.1 - Section 1 Meet New Agency
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
  
</style>