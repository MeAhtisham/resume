<template>
  <div class="product-card">
    <div class="product-img">
      <img :src="product.img" alt="" class="img-fluid" />
    </div>
    <div class="product-info">
      <div>
        <img :src="plus" alt="" class="img-fluid" />
        <p>{{ product.title }}</p>
        <p>shop it now</p>
      </div>
    </div>
    <div class="overlay"> </div>
  </div>
</template>

<script>
import plus from "../assets/plus.svg";
export default {
  props: {
    product: {
      type: Object,
    },
  },
  data() {
    return {
      plus,
    };
  },
};
</script>

<style>
.product-card {
  position: relative;
  /* box-shadow: 12px 12px 2px 1px rgba(0, 0, 255, 0.2); */
}
.product-card:hover .product-info {
  opacity: 1;
}
.product-info {
  text-align: center;
  position: absolute;
  top: 0;
  bottom: 0;
  right: 0;
  left: 0;
  margin: auto;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: rgba(0, 0, 0, 0.5);
  opacity: 0;
  transition: ease-in-out all 0.5s;
  cursor: pointer;
}

.product-info img {
  width: 20px;
}
.product-info p {
  color: white;
  margin: 0;
}
/* .overlay {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  margin: auto;
  background-color: rgb(5, 4, 4);
  opacity: 0.5;
} */
</style>
