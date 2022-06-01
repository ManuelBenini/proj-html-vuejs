<template>

  <div class="courses">
    <div class="mb-container">

      <div class="text-center">
        <SectionTitle 
          title="CHOOSE A COURSE TO GET STARTED" 
          firstText="Latest Featured" 
          coloredText="Courses"
        />
      </div>

      <div class="mb-course-cards-container d-flex flex-wrap">

        <CourseCard 
          imageNumber="1" 
          coloredIntegerPrice="$40"
          coloredDecimalPrice=".00"
          courseDescription="Learning to Write as a Professional Author"
          lessons="20"
          students="50" 
        />

        <CourseCard 
          imageNumber="2" 
          coloredIntegerPrice="free"
          courseDescription="Customer-centric Info-Tech Strategies"
          lessons="24"
          students="769" 
        />

        <CourseCard 
          imageNumber="3" 
          coloredIntegerPrice="$19"
          coloredDecimalPrice=".00"
          courseDescription="Open Programming courses for Everyone: Python"
          lessons="17"
          students="62" 
        />

        <CourseCard 
          imageNumber="4" 
          coloredIntegerPrice="$26"
          coloredDecimalPrice=".00"
          courseDescription="Academic Listening and Note-taking"
          lessons="14"
          students="67" 
        />

        <CourseCard 
          imageNumber="5" 
          coloredIntegerPrice="$39"
          coloredDecimalPrice=".00"
          courseDescription="Master jQuery in a Short Period of Time"
          lessons="6"
          students="51" 
        />

        <CourseCard 
          imageNumber="6" 
          coloredIntegerPrice="$59"
          coloredDecimalPrice=".00"
          courseDescription="Introduction to Javascript for Beginners"
          lessons="14"
          students="76" 
        />

      </div>

      <div class="courses-btn text-center">
        <AccentBtnComp class="blackHoveredBtn" style="padding: 16px 65px;" btnText='View all courses' />
      </div>

    </div>
  </div>
  
</template>

<script>
  import CourseCard from './CourseCard.vue';
  import SectionTitle from './SectionTitle.vue';
  import AccentBtnComp from './AccentBtnComp.vue';

  export default {
    name: 'CoursesComp',
    components: {CourseCard, SectionTitle, AccentBtnComp}
  }
</script>

<style lang="scss" scoped>
  @import '../assets/style/variables';

  .courses{
    padding: 100px 0;
    background-color: $sections-color;
    .mb-container{
      .courses-btn{
        margin-top: 50px;
        .blackHoveredBtn:hover{
          background-color: #3f3a64;
          color: white;
        } 
      }
    }
  }

</style>