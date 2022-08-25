<template>
  <div>
    <Contactus />
    <ContactData />
    <ContactForm/>
    <Map />
    <Footer />
  </div>
</template>

<script>
import Footer from "../components/Footer.vue"
import Contactus from "../components/Contactus.vue"
import ContactData from "@/components/ContactData.vue";
import Map from "@/components/Map.vue";
import ContactForm from "@/components/ContactForm.vue";
export default {
  name: "Home",
  components: {
    Footer,
    Contactus,
    Map,
    ContactData,
    ContactForm
},
};
</script>

<style scoped>
</style>

