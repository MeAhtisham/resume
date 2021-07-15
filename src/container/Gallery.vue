<template>
  <section id="gallery">
    <b-container>
      <b-row>
        <b-col md="5" offset-md="1">
          <Theamtitle heading="ardad" subheading="rana"></Theamtitle>
        </b-col>
        <b-col md="5" offset-md="1">
          <b-btn @click="handleKeys('all')">all</b-btn>
          <b-btn @click="handleKeys('cate1')">cate1</b-btn>
          <b-btn @click="handleKeys('cate2')">cate2</b-btn>
          <b-btn @click="handleKeys('cate3')">cate3</b-btn>
        </b-col>
      </b-row>
      <b-row>
        <b-col
          class="mb-4"
          md="4"
          v-for="product in products"
          :key="product.id"
        >
          <ProductCard :product="product" />
        </b-col>
      </b-row>
    </b-container>
  </section>
</template>

<script>
import ProductCard from "../components/ProductCard.vue";
import Theamtitle from "../components/Theamtitle.vue";
import img from "../assets/1.jpg";
const productsList = [
  {
    id: 1,
    category: "cate1",
    title: "title 1",
    img,
  },
  {
    id: 2,
    category: "cate2",
    title: "title 2",
    img,
  },
  {
    id: 3,
    category: "cate3",
    title: "title 3",
    img,
  },
  {
    id: 4,
    category: "cate2",
    title: "title 4",
    img,
  },
  {
    id: 5,
    category: "cate1",
    title: "title 5",
    img,
  },
  {
    id: 6,
    category: "cate1",
    title: "title 6",
    img,
  },
];
export default {
  data() {
    return {
      products: [],
    };
  },
  methods: {
    handleKeys(key) {
      switch (key) {
        case "all":
          return (this.products = productsList);
        case "cate1":
          return (this.products = productsList.filter(
            (product) => key === product.category
          ));
        case "cate2":
          return (this.products = productsList.filter(
            (product) => key === product.category
          ));
        case "cate3":
          return (this.products = productsList.filter(
            (product) => key === product.category
          ));
        default:
          this.products;
      }
    },
  },
  components: { Theamtitle, ProductCard },
  mounted() {
    console.log("hello");
    this.handleKeys("all");
  },
};
</script>

<style>
#gallery {
  padding: 60px 0px;
}
</style>
