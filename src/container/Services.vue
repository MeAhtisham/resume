<template>
  <section id="services">
    <b-container>
      <b-row align-h="center">
        <b-col md="10">
          <b-row>
            <b-col md="12">
              <Theamtitle
                heading="my services"
                subheading="Service i provide"
                className="light"
              ></Theamtitle>
            </b-col>
          </b-row>
        </b-col>
      </b-row>
      <b-row align-h="center">
        <b-col md="10">
          <b-row>
            <b-col md="4" v-for="(service, index) in services" :key="index">
              <Servicecard
                :title="service.title"
                :subtitle="service.subtitle"
                :img="service.img"
              ></Servicecard>
            </b-col>
          </b-row>
        </b-col>
      </b-row>
    </b-container>
  </section>
</template>

<script>
import Servicecard from "../components/Servicecard.vue";
import Theamtitle from "../components/Theamtitle.vue";
import advertising from "../assets/advertising.svg";
import camera from "../assets/camera.svg";
import like from "../assets/like.svg";
import server from "../assets/server.svg";
import settings from "../assets/settings.svg";
import web from "../assets/web-programming.svg";
export default {
  components: {
    Servicecard,
    Theamtitle,
  },
  data() {
    return {
      services: [
        {
          img: server,
          title: "web development",
          subtitle:
            "Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quasi veroipsa in sint quo nobis minima beatae dicta! Expedita quos veritatisincidunt hic, voluptates reiciendis aliquid deleniti dolore debitismaiores!",
        },
        {
          img: web,
          title: "web development",
          subtitle:
            "Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quasi veroipsa in sint quo nobis minima beatae dicta! Expedita quos veritatisincidunt hic, voluptates reiciendis aliquid deleniti dolore debitismaiores!",
        },
        {
          img: camera,
          title: "web development",
          subtitle:
            "Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quasi veroipsa in sint quo nobis minima beatae dicta! Expedita quos veritatisincidunt hic, voluptates reiciendis aliquid deleniti dolore debitismaiores!",
        },
        {
          img: advertising,
          title: "web development",
          subtitle:
            "Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quasi veroipsa in sint quo nobis minima beatae dicta! Expedita quos veritatisincidunt hic, voluptates reiciendis aliquid deleniti dolore debitismaiores!",
        },
        {
          img: settings,
          title: "web development",
          subtitle:
            "Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quasi veroipsa in sint quo nobis minima beatae dicta! Expedita quos veritatisincidunt hic, voluptates reiciendis aliquid deleniti dolore debitismaiores!",
        },
        {
          img: like,
          title: "web development",
          subtitle:
            "Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quasi veroipsa in sint quo nobis minima beatae dicta! Expedita quos veritatisincidunt hic, voluptates reiciendis aliquid deleniti dolore debitismaiores!",
        },
      ],
    };
  },
};
</script>

<style>
#services {
  background-color: black;
  padding: 60px 0px;
}
</style>
