<template>
  <div :class="e - card - body">
    <img :src="img" alt="" class="img-fluid" />
    <div :class="`e-card-fotter ${classclr}`">
      <h2 v-if="title1">{{ title1 }}</h2>
      <h2>{{ title }}</h2>
      <p>{{ subtitle }}</p>
      <h2 v-if="subtitle1">{{ subtitle1 }}</h2>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    img: String,
    title: String,
    subtitle: String,
    title1: String,
    subtitle1: String,
    classclr: String,
  },
};
</script>

<style>
.e-card-body {
  /* height: 40px; */
  box-shadow: 0px 0px 5px 0px #fbfbfb;
  margin-top: 20px !important;
}
.e-card-fotter h2 {
  margin-bottom: 5px !important;
  margin-top: 15px !important;
  font-weight: bold !important;
}
.e-card-body img {
  min-height: 196px !important;
}
.e-card-fotter {
  padding: 15px;
  background-color: white;
}
.clr {
  background-color: black !important;
}
</style>
