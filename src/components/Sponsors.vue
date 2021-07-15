<template>
  <div class="company-logo">
    <img :src="img" alt="" class="img-fluid" />
  </div>
</template>

<script>
export default {
  props: {
    img: String,
  },
};
</script>

<style></style>
