<template>
  <div id="app">
    <HeaderSection></HeaderSection>
    <Aboutme></Aboutme>
    <Counter></Counter>
    <Gallery />
    <Education></Education>
    <Services></Services>
    <Sponsorssec></Sponsorssec>
  </div>
</template>
<script>
import HeaderSection from "./container/HeaderSection";
import Aboutme from "./container/Aboutme.vue";
import Counter from "./container/CounterSec.vue";
import Gallery from "./container/Gallery.vue";
import Education from "./container/Education.vue";
import Services from "./container/Services.vue";
import Sponsorssec from "./container/Sponsorssec.vue";
// import HelloWorld from "./components/HelloWorld";
export default {
  components: {
    HeaderSection,
    Aboutme,
    Counter,
    Gallery,
    Education,
    Services,
    Sponsorssec,
    // Card,
    // Hell
    // oWorld,
  },
  data() {
    return {
      hed: "i am heading you just creatred using props",
      para: "i am paara",
    };
  },
};
</script>

<style></style>
