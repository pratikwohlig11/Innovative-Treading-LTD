<template>
  <div>
    <Aboutimg/>
    <Aboutbio/>
    <Afooter />
  </div>
</template>

<script>
import Afooter from "../components/Afooter.vue"
import Aboutimg from "@/components/Aboutimg.vue"
import Aboutbio from "@/components/Aboutbio"

export default {
  name: "Home",
  components: {
    Afooter,
    Aboutimg,
    Aboutbio,
},
};
</script>

<style scoped>
</style>

