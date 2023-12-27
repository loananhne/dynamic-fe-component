<template>
  <NavBar />
  <Hero />
  <About />
  <WhyUs />
  <StatsCounter />
  <MenuAll />
  <Testimonials />
  <Contact />
  <Footer />
</template>

<script>
import Hero from "./Hero.vue";
import NavBar from "./NavBar.vue";
import Catalog from "./Catalog.vue";
import About from "./About.vue";
import WhyUs from "./WhyUs.vue";
import StatsCounter from "./StatsCounter.vue";
import MenuAll from "./MenuAll.vue";
import Testimonials from "./Testimonials.vue";
import Contact from "./Contact.vue";
import Footer from "./Footer.vue";

export default {
  components: {
    Hero,
    NavBar,
    Catalog,
    About,
    WhyUs,
    StatsCounter,
    MenuAll,
    Testimonials,
    Contact,
    Footer,
  },
};
</script>

<style></style>
