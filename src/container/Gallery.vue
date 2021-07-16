<template>
  <section id="gallery">
    <b-container>
      <b-row align-h="center" align-v="center">
        <b-col md="10">
          <b-row>
            <b-col cols="12" md="6">
            <Theamtitle heading="my work ____________" subheading="project i have done" classmb="mb"></Theamtitle>
            </b-col>
            <b-col cols="12" md="6" >
              <div class="btncls">
          <b-btn @click="handleKeys('all')">all</b-btn>
          <b-btn @click="handleKeys('cate1')">cate1</b-btn>
          <b-btn @click="handleKeys('cate2')">cate2</b-btn>
          <b-btn @click="handleKeys('cate3')">cate3</b-btn>
              </div>
           
        </b-col>
          </b-row>

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
import coin from "../assets/coin.jpg";
import tree from "../assets/tree.jpg";
// import shoes from "../assets/shoes.jpg";
import shirt from "../assets/shirt.jpg";
// import coin from "../assets/coin.jpg";
// import coin from "../assets/coin.jpg";
const productsList = [
  {
    id: 1,
    category: "cate1",
    title: "title 1",
    img:coin
  },
  {
    id: 2,
    category: "cate2",
    title: "title 2",
    img:tree
  },
  {
    id: 3,
    category: "cate3",
    title: "title 3",
    img:shirt
  },
  {
    id: 4,
    category: "cate2",
    title: "title 4",
    img:coin
  },
  {
    id: 5,
    category: "cate1",
    title: "title 5",
    img:shirt
  },
  {
    id: 6,
    category: "cate1",
    title: "title 6",
    img:tree
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
.btn-secondary{
  margin-right:  15px !important;
}
</style>
