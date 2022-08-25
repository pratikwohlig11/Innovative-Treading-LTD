<template>
  <div>
    <Aboutimg/>
    <Aboutbio/>
    <Footer />
  </div>
</template>

<script>
import Footer from "../components/Footer.vue"
import Aboutimg from "@/components/Aboutimg.vue"
import Aboutbio from "@/components/Aboutbio"

export default {
  name: "Home",
  components: {
    Footer,
    Aboutimg,
    Aboutbio,
},
};
</script>

<style scoped>
</style>

