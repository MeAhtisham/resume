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
          <Counter
            :title="count.title"
            :subtitle="count.subtitle"
            :img="count.image"
          ></Counter>
        </b-col>
      </b-row>
    </b-container>
  </section>
</template>

<script>
import Counter from "../components/Counter.vue";
import image from "../assets/ice-cream.svg";
import heart from "../assets/heart.svg";
import coffee from "../assets/coffee-cup.svg";
export default {
  components: {
    Counter,
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
