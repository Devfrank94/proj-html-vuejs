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
      <div class="fmcontainer test">
        <div class="title-cont d-flex flex-dir-col al-item-cent">
          <h3 class="mt-5 mb-4">meet the new agency SEO template<br>from the avada team</h3>
          <p class="mb-5">Lorem ipsum dolor sit amet consectetur adipisicing elit. <br> Dolor, nam voluptas dolorum placeat libero itaque?</p>
        </div>

      </div>

    </section>
















  </main>

  
</template>


<style lang="scss" scoped>

  @use '../scss/main.scss' as *;

  // 2. Main
  // - 2.1 - Section 1 Meet New Agency
  section:nth-child(odd){
    background-color: $bg-sect;
    height: 400px; //da rimuovere
  }

  .title-cont{

    h3{
    font-size: 1.3rem;
    font-weight: 700;
    }

    p{
      font-size: .8rem;
      color: $gray;
    }
  }

</style>