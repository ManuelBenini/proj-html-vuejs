<template>

  <main>
    
    <HeroComp />

    <AchievementComp />

    <ServicesComp />

    <CoursesComp />

    <TestimonialsComp />

    <BlogsComp />

    <LearnCategoriesComp />

    <CallToActionComp />

  </main>
  
</template>

<script>
  import ServicesComp from './ServicesComp.vue';
  import HeroComp from './HeroComp.vue';
  import AchievementComp from './AchievementComp.vue';
  import CoursesComp from './CoursesComp.vue';
  import TestimonialsComp from './TestimonialsComp.vue';
  import BlogsComp from './BlogsComp.vue';
  import LearnCategoriesComp from './LearnCategoriesComp.vue';
  import CallToActionComp from './CallToActionComp.vue';


  export default {
    name: "MainComp",
    components: { ServicesComp, HeroComp, AchievementComp, CoursesComp, TestimonialsComp, BlogsComp, LearnCategoriesComp, CallToActionComp }
  }
  
</script>

<style lang="scss" scoped>
  @import '../assets/style/variables';  

</style>