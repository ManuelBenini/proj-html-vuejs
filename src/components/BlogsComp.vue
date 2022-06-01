<template>

  <div class="blogs">

    <div class="mb-container">

      <div class="text-center">
        <SectionTitle title="ENJOY READING ON MAXCOACH" firstText="Latest on" coloredText="Our Blogs" />
      </div>

      <div class="mb-cards-container mt-5 d-flex">

        <BlogCard 
          image="artist-blog-03-480x325" 
          :isImageJpeg="true"
          artist="ARTIST" 
          blogTitle="Brush Strokes Energize Trees In Paintings"
          date="May 15, 2020" views="688"
        />

        <BlogCard 
          image="artist-blog-01-480x325" 
          :isImageJpeg="false"
          artist="ARTIST" 
          blogTitle="Pocket-Sized Notebooks Hold Miniature Paintings"
          date="May 15, 2020" views="603"
        />

        <BlogCard 
          image="artist-blog-02-480x325" 
          :isImageJpeg="false"
          artist="ARTIST" 
          blogTitle="Connection Between Self-Portraits and Identity"
          date="May 15, 2020" views="397"
        />

      </div>

    </div>
  </div>
  
</template>

<script>
  import SectionTitle from './SectionTitle.vue';
  import BlogCard from './BlogCard.vue';

  export default {
    name: 'TestimonialsComp',
    components: {SectionTitle, BlogCard}
  }
  
</script>

<style lang="scss" scoped>
  @import '../assets/style/variables';

  .blogs{
    padding: 70px 0;
    background-color: $sections-color;
  }

</style>