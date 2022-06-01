<template>

  <div class="services">
      <div class="mb-container d-flex">

        <div class="mb-columns d-flex">

          <div class="mb-column mb-column-1">

            <ServicesCard 
              title="Graphic Design"
              text="Have a passion for graphics and arts? Show your talents with confidence and self-assertiveness." 
              imageNumber="1"
              :inverse="false"
            />

            <ServicesCard 
              title="Idea Discussion"
              text="Get teamed up with the specialists who work and teach coding for years at famous universities" 
              imageNumber="3"
              :inverse="true"
            />

          </div>
  
         <div class="mb-column mb-column-2">

            <ServicesCard 
              title="Business Administration"
              text="Leaners are encouraged to study the mechanism and structure of system administation." 
              imageNumber="2"
              :inverse="false" 
            />

            <ServicesCard 
              title="Web Development"
              text="Learn to start building a webpage from scatch. you decide your own pace, course and speed." 
              imageNumber="4"
              :inverse="true"
            />

          </div>

        </div>

        <div class="services-to-create">

          <SectionTitle 
            title="TOGETHER WE CAN CREATE" 
            firstText="Services We" 
            coloredText="Can Provide" 
            secondText="For My Clients." 
          />

          <div class="options mt-5">
            <CheckboxComp text="Select & customize courses to your preferences" />
            <CheckboxComp text="Change the tutor and make arrangements" />
            <CheckboxComp text="Partecipate in events to join others" />
            <CheckboxComp text="Get the desired certificate delivered at house" />
          </div>

          <AccentBtnComp class="mt-3 blackHoveredBtn" btnText="Get started for free" />

        </div>

      </div>
    </div>
  
</template>

<script>
  import CheckboxComp from './CheckboxComp.vue';
  import ServicesCard from './ServicesCard.vue';
  import SectionTitle from './SectionTitle.vue';
  import AccentBtnComp from './AccentBtnComp.vue';

  export default {
    name: 'ServicesComp',
    components: {CheckboxComp, ServicesCard, SectionTitle, AccentBtnComp }
  }

</script>

<style lang="scss" scoped>
  @import '../assets/style/variables';

  .services{
    .mb-container{
      padding-top: 130px;
      padding-bottom: 60px;
      background-image: url('../assets/img/background-pattern-grid-line.png');
      background-size: 331px 100px;
    }
    .mb-column{
      width: 250px;
      margin-right: 15px;
    }
    .mb-column-2{
      margin-top: 50px;
      margin-left: 10px;
    }
    .services-to-create{
      padding-top: 175px;
      margin-left: 52px;
      width: 380px;
      .blackHoveredBtn:hover{
        background-color: #3f3a64;
        color: white;
      }
    }
  }

</style>