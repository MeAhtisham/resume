<template>
  <div>
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
  },
};
</script>

<style>
.theme-subheading {
  font-weight: bold;
  color: black;
  font-size: 35px;
  text-transform: capitalize;
}
</style>
