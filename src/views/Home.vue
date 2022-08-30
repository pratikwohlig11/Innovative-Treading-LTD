<template>
  <div>
    <Slider />
    <Eyn />
    <Sa />
    <Footer />
  </div>
</template>

<script>
import Footer from "../components/Footer.vue";
import Slider from "../components/Slider.vue";
import Eyn from "../components/Eyn.vue";
import Sa from "../components/Sa.vue";
export default {
  name: "Home",
  components: {
    Footer,
    Slider,
    Eyn,
    Sa,
  },
};
</script>

<style scoped>
</style>

