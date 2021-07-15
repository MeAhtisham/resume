<template>
  <div class="s-card-head">
    <img :src="img" alt="" class="img-fluid" />
    <div class="s-card-footer">
      <h2>{{ title }}</h2>
      <p>{{ subtitle }}</p>
    </div>
  </div>
</template>
<script>
export default {
  props: {
    img: String,
    title: String,
    subtitle: String,
  },
};
</script>

<style>
.s-card-head img {
  width: 40px;
}
.s-card-head {
  margin-top: 10px;
}
.s-card-footer h2 {
  text-transform: capitalize;
  margin-bottom: 0 !important;
  margin-top: 10px;
  color: white !important;
}
.s-card-footer p {
  color: white;
  margin-top: 10px;
}
.s-card-footer {
  margin-top: 20px;
}
</style>
