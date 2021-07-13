<template>
  <b-button :variant="variant">{{ btnTxt }}</b-button>
</template>

<script>
export default {
  props: {
    variant: String,
    btnTxt: String,
  },
};
</script>

<style>
.btn-primary {
  background-color: #3e3e3e !important;
  border: none !important;
  padding: 10px 25px !important;
  margin-top: 15px;
}
.btn-secondary {
  background-color: white;
  color: red;
}
</style>
