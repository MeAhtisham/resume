<template>
  <section id="aboutus">
    <b-container>
      <b-row>
        <b-col lg="10">
          <b-row class="justify-content-md-center" align-v="center">
            <b-col lg="6" sm="12">
              <img src="../assets/1.jpg" alt="" class="img-fluid" />
            </b-col>
            <b-col lg="6" sm="12">
              <Theamtitle
                heading="me Ahtisham"
                subheading="My name is Ahtisham
            i am a expert in web design & web
           develpoment"
              ></Theamtitle>

              <p
                >Lorem ipsum dolor sit amet consectetur adipisicing elit.
                Mollitia, est! Sit iste aspernatur, laboriosam a aliquid
                necessitatibus, consequatur nesciunt ab tenetur reiciendis
                accusamus, totam minima! Iure vel quia sed laudantium.</p
              >
              <b-row>
                <b-col
                  cols="4"
                  md="4"
                  v-for="(content, ind) in cardcontent"
                  :key="ind"
                >
                  <AppCard
                    :title="content.title"
                    :subtitle="content.subtitle"
                    :img="content.image"
                  ></AppCard>
                </b-col>
              </b-row>
              <Button variant="primary" btnTxt="read more"></Button>
            </b-col>
          </b-row>
        </b-col>
      </b-row>
    </b-container>
  </section>
</template>

<script>
import Theamtitle from "../components/Theamtitle.vue";
import Button from "../components/Button.vue";
import AppCard from "../components/AppCard.vue";
import image from "../assets/photoshop-logo.svg";
export default {
  components: {
    Theamtitle,
    Button,
    AppCard,
  },
  data() {
    return {
      cardcontent: [
        {
          title: "Abod",
          subtitle: "photoshop",
          image,
        },
        {
          title: "Abod",
          subtitle: "photoshop",
          image,
        },
        {
          title: "Abod",
          subtitle: "photoshop",
          image,
        },
      ],
    };
  },
};
</script>

<style scoup>
#aboutus {
  padding-top: 40px;
  padding-bottom: 40px;
}
</style>
