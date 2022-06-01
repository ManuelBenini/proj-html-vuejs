<template>

  <div class="call-to-action position-relative">

    <div class="circles">
      <div class="yellow-fill"></div>
      <div class="pink-fill"></div>
      <div class="azure-fill"></div>
    </div>

    <div class="mb-container text-center">

      <h5>Start today for getting <ColoredTextComp text="Online Certification" /></h5>
      <h2 class="mb-4">You can be your own guiding star with our help!</h2>
      <AccentBtnComp class="blackHoveredBtn" style="padding: 16px 65px;" btnText="Get started now" />

    </div>

  </div>
  
</template>

<script>
  import AccentBtnComp from './AccentBtnComp.vue';
  import ColoredTextComp from './ColoredTextComp.vue';

  export default {
    name: "TestimonialsComp",
    components: { AccentBtnComp, ColoredTextComp }
  }
</script>

<style lang="scss" scoped>
  @import '../assets/style/variables';

  .call-to-action{
    padding: 100px 0;
    .blackHoveredBtn:hover{
      background-color: #3f3a64;
      color: white;
    } 
    .circles{
      & *{
        position: absolute;
        border-radius: 50%;
        border: 1px solid
      }
      .yellow-fill{
        top: 150px;
        left: 120px;
        width: 40px;
        height: 40px;
        background-color: #ebb860;
        border-color: #e7ab37;
      }
      .pink-fill{
        top: 5px;
        left: 1430px;
        width: 35px;
        height: 35px;
        background-color: #e88c98;
        border-color: #e37283;
      }
      .azure-fill{
        bottom: 175px;
        left: 1670px;
        width: 35px;
        height: 35px;
        background-color: #aab8f1;
        border-color: #9fafef;
      }
    }
  }

</style>