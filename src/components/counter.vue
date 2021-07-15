<template>
  <div class="counter-content">
    <img :src="img" alt="" class="img-fluid" />
    <h2>{{ title }}</h2>
    <p>{{ subtitle }}</p>
  </div>
</template>

<script>
export default {
  props: {
    title: String,
    subtitle: String,
    img: String,
  },
};
</script>

<style scoped>
.counter-content {
  text-align: center;
}
.counter-content img {
  width: 60px;
}
.counter-content h2 {
  margin: 0px !important;
  padding-top: 16px !important;
  font-weight: 900 !important;
  color: black !important;
}
.counter-content {
  text-transform: capitalize;
}
</style>
