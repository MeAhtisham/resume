<template>
  <section id="counter">
    <b-container>
      <b-row align-v="center">
        <b-col
          cols="12"
          sm="6"
          md="3"
          v-for="(count, index) in counter1"
          :key="index"
        >
          <counter
            :title="count.title"
            :subtitle="count.subtitle"
            :img="count.image"
          ></counter>
        </b-col>
      </b-row>
    </b-container>
  </section>
</template>

<script>
import counter from "../components/counter.vue";
import image from "../assets/ice-cream.svg";
import heart from "../assets/heart.svg";
import coffee from "../assets/coffee-cup.svg";
export default {
  components: {
    counter,
  },
  data() {
    return {
      counter1: [
        {
          title: "3265",
          subtitle: "project completed",
          image: image,
        },
        {
          title: "5265",
          subtitle: "cup of coffee",
          image: coffee,
        },
        {
          title: "3265",
          subtitle: "project completed",
          image: heart,
        },
        {
          title: "3265",
          subtitle: "project completed",
          image,
        },
      ],
    };
  },
};
</script>

<style>
#counter {
  padding: 100px 0px;
  background-color: #f8f7fd;
}
</style>
