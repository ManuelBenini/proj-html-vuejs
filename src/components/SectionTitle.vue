<template>

  <div>
    <p>{{title}}</p>
    <h1>{{firstText}} <ColoredTextComp :text="coloredText" /> {{secondText? secondText : ''}}</h1>
  </div>

</template>

<script>
import ColoredTextComp from './ColoredTextComp.vue';
export default {
    name: "SectionTitle",
    props: {
      title: String,
      firstText: String,
      secondText: String,
      coloredText: String
    },
    components: { ColoredTextComp }
}
</script>

<style lang="scss" scoped>
  @import '../assets/style/variables';

  p{
    font-family: "atma";
  }

</style>