<template>
  <div :class="`theme-title-default ${className}`">
    <p class="theme-heading"> {{ heading }}</p>
    <h2 class="theme-subheading">
      {{ subheading }}
    </h2>
  </div>
</template>

<script>
export default {
  props: {
    heading: String,
    subheading: String,
    className: String,
  },
};
</script>

<style>
.theme-title-default h2 {
  font-weight: bold;
  color: black;
  font-size: 25px !important;
  text-transform: uppercase;
}
.theme-title-default p {
  margin-bottom: 5px !important;
  color: black;
}
.light h2,
.light p {
  color: #fff !important;
}
</style>
