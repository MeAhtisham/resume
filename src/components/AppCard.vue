<template>
  <div class="theme-card">
    <img height="50px" :src="img" class="img-fluid" :alt="img || test" />
    <div :class="`theme-body ${classml}`">
      <p>{{ title || "no title" }}</p>
      <h2>{{ subtitle || "no subtitle" }}</h2>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: String,
    subtitle: String,
    img: String,
    classml: String,
  },
};
</script>

<style>
.theme-card {
  display: flex;
  margin-top: 10px;
}
.theme-card img {
  height: 50px !important;
}
h2 {
  font-size: 14px !important;
  font-weight: bold !important;
  color: rgba(32, 30, 30, 0.87) !important;
}
.theme-body p {
  font-size: 12px;
  font-weight: 500;
  color: #6f6f6f;
  margin-bottom: 0;
  padding-top: 5px;
}
/* .theme-body {
  margin-left: 10px;
} */
.ml {
  margin-left: 10px;
}
</style>
