<template>
  <div>
    <b-button :variant="variant" :class="btncls">{{ btnTxt }}</b-button>
  </div>
</template>

<script>
export default {
  props: {
    variant: String,
    btnTxt: String,
    btncls: String,
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
.newbtn {
  background-color: black !important;
  margin-top: 20px !important;
}
</style>
