<template>
  <section id="education">
    <b-container>
      <b-row align-h="center">
        <b-col md="10">
          <b-row>
            <b-col md-12>
              <Theamtitle
                heading="my experience"
                subheading="education & experience"
              >
              </Theamtitle>
            </b-col>
          </b-row>
        </b-col>
      </b-row>
      <b-row align-h="center">
        <b-col md="10">
          <b-row>
            <b-col md="4" v-for="(content, index) in contents" :key="index">
              <Educationcard
                :title="content.title"
                :subtitle="content.subtitle"
                :img="content.img"
              ></Educationcard>
            </b-col>
          </b-row>
        </b-col>
      </b-row>
      <b-row>
        <b-col cols="12">
          <div class="btn-center">
            <Button variant="primary" btnTxt=" download more" />
          </div>
        </b-col>
      </b-row>
    </b-container>
  </section>
</template>

<script>
import Educationcard from "../components/Educationcard.vue";
import Theamtitle from "../components/Theamtitle.vue";
import img1 from "../assets/1.jpg";
import img2 from "../assets/2.jpg";
import img3 from "../assets/3.jpg";
import img4 from "../assets/4.jpg";
import img5 from "../assets/5.jpg";
import Button from "../components/Button.vue";
// import img6 from "../assets/6.jpg";
export default {
  components: { Theamtitle, Educationcard, Button },
  data() {
    return {
      contents: [
        {
          img: img1,
          title: "Education and Experience",
          subtitle:
            "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Amet liberoipsa consectetur impedit quasi unde. Ipsa dolorum obcaecati in quia. Facere odio vitae, expedita dicta numquam eligendi autem? Vel, iste!",
        },
        {
          img: img2,
          title: "Education and Experience",
          subtitle:
            "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Amet liberoipsa consectetur impedit quasi unde. Ipsa dolorum obcaecati in quia. Facere odio vitae, expedita dicta numquam eligendi autem? Vel, iste!",
        },
        {
          img: img3,
          title: "Education and Experience",
          subtitle:
            "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Amet liberoipsa consectetur impedit quasi unde. Ipsa dolorum obcaecati in quia. Facere odio vitae, expedita dicta numquam eligendi autem? Vel, iste!",
        },
        {
          img: img4,
          title: "Education and Experience",
          subtitle:
            "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Amet liberoipsa consectetur impedit quasi unde. Ipsa dolorum obcaecati in quia. Facere odio vitae, expedita dicta numquam eligendi autem? Vel, iste!",
        },
        {
          img: img5,
          title: "Education and Experience",
          subtitle:
            "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Amet liberoipsa consectetur impedit quasi unde. Ipsa dolorum obcaecati in quia. Facere odio vitae, expedita dicta numquam eligendi autem? Vel, iste!",
        },
        {
          img: img4,
          title: "Education and Experience",
          subtitle:
            "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Amet liberoipsa consectetur impedit quasi unde. Ipsa dolorum obcaecati in quia. Facere odio vitae, expedita dicta numquam eligendi autem? Vel, iste!",
        },
      ],
    };
  },
};
</script>

<style>
.btn-center {
  text-align: center;
  /* margin-top: 45px; */
}
#education {
  background-color: #ededed;
  padding-bottom: 85px;
  padding-top: 85px;
}
</style>
