<template>
  <div id="app">
    <HeaderSection></HeaderSection>
    <Aboutme></Aboutme>
  </div>
</template>
<script>
import HeaderSection from "./container/HeaderSection";
import Aboutme from "./container/Aboutme.vue";
// import HelloWorld from "./components/HelloWorld";
export default {
  components: {
    HeaderSection,
    Aboutme,
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
