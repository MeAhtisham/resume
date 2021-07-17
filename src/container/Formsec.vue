<template>
  <section id="form1">
    <b-container>
      <b-row align-h="center">
        <b-col md="10">
          <b-row>
            <b-col md="4" v-for="(card, index) in cards" :key="index">
              <AppCard
                :title="card.title"
                :subtitle="card.subtitle"
                :img="card.img"
                classml="ml"
              ></AppCard>
            </b-col>
            <b-col class="form-heading">
              <h2>leave a message</h2>
            </b-col>
          </b-row>
          <b-row>
            <b-col md="4">
              <div><label for="">Name</label></div>
              <input type="text" name="Name" id="" />
            </b-col>
            <b-col md="4">
              <div><label for="">Email</label></div>
              <input type="text" name="Name" id="" />
            </b-col>
            <b-col md="4">
              <div><label for="">phone</label></div>
              <input type="text" name="Name" id="" />
            </b-col>
            <b-col col="12" sm="12">
              <div><label for="">message</label></div>
              <input class="full" type="text" name="Name" id="" />
            </b-col>
            <b-col cols="12">
              <Button
                variant="primary"
                btnTxt="send message"
                btncls="newbtn"
              ></Button>
            </b-col>
          </b-row>
        </b-col>
      </b-row>
    </b-container>
  </section>
</template>

<script>
import AppCard from "../components/AppCard.vue";
import headphone from "../assets/headphone.svg";
import pin from "../assets/pin.svg";
import Button from "../components/Button.vue";
export default {
  components: { AppCard, Button },
  data() {
    return {
      cards: [
        {
          title: "cell phone",
          subtitle: "034454545454",
          img: pin,
        },
        {
          title: "contact us",
          subtitle: "333434",
          img: headphone,
        },
        {
          title: "location",
          subtitle: "gilgit pakistan",
          img: pin,
        },
      ],
    };
  },
};
</script>

<style scoped>
.full {
  width: 100%;
  margin-top: 30px;
}
#form1 {
  padding: 81px 0px !important;
}
.form-heading {
  margin-top: 20px !important;
}
.form-heading h2 {
  font-size: 22px !important;
  font-weight: bold !important;
  text-transform: capitalize;
}
input {
  border-top-style: hidden;
  border-right-style: hidden;
  border-left-style: hidden;
  text-decoration: none;
  border-radius: 1px solid black;
  outline: none;
  width: 100%;
}
label {
  margin-top: 20px;
}
</style>
