<template>
  <section id="sponsrs">
    <b-container>
      <b-row align-h="center">
        <b-col md="10">
          <b-row>
            <b-col
              cols="6"
              md="2"
              v-for="(image, index) in content"
              :key="index"
            >
              <div class="mtt">
                <Sponsors :img="image.img" alt="s"></Sponsors>
              </div>
            </b-col>
            <div class="hr">
              <hr />
            </div>
          </b-row>
        </b-col>
      </b-row>
      <b-row align-h="center">
        <b-col cols="12" sm="12" md="10">
          <b-row>
            <b-col md="4" v-for="(card, index) in cards" :key="index">
              <Educationcard
                :title="card.title"
                :subtitle="card.subtitle"
                :img="card.img"
                :subtitle1="card.subtitle1"
                :title1="card.title1"
                :classclr="clr"
              ></Educationcard>
            </b-col>
          </b-row>
        </b-col>
      </b-row>
    </b-container>
  </section>
</template>

<script>
import Sponsors from "../components/Sponsors.vue";

import logo from "../assets/v.png";
import Educationcard from "../components/Educationcard.vue";
import img2 from "../assets/2.jpg";
import img3 from "../assets/3.jpg";
import img4 from "../assets/4.jpg";
export default {
  components: { Sponsors, Educationcard },
  data() {
    return {
      content: [
        {
          img: logo,
        },
        {
          img: logo,
        },
        {
          img: logo,
        },
        {
          img: logo,
        },
        {
          img: logo,
        },
        {
          img: logo,
        },
      ],
      cards: [
        {
          img: img2,
          title1: "rana",
          title: "Discove the world",
          subtitle:
            "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Amet liberoipsa consectetur impedit quasi unde. Ipsa dolorum obcaecati in quia. Facere odio vitae, expedita dicta numquam eligendi autem? Vel, iste!",
          subtitle1: "read more",
        },
        {
          img: img3,
          title1: "rana",
          title: "beautifl world",
          subtitle:
            "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Amet liberoipsa consectetur impedit quasi unde. Ipsa dolorum obcaecati in quia. Facere odio vitae, expedita dicta numquam eligendi autem? Vel, iste",
          subtitle1: "read more",
        },
        {
          img: img4,
          title1: "rana",
          title: "think outside the box",
          subtitle:
            "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Amet liberoipsa consectetur impedit quasi unde. Ipsa dolorum obcaecati in quia. Facere odio vitae, expedita dicta numquam eligendi autem? Vel, iste!",
          subtitle1: "read more",
        },
      ],
    };
  },
};
</script>

<style>
#sponsrs {
  background-color: #f8f7fd;
  padding: 60px;
  padding: 6opx;
}
.hr {
  margin-top: 25px !important;
  margin-bottom: 20px !important;
}

.mtt {
  margin-top: 10px;
}
</style>
