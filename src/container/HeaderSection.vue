<template>
  <section id="header-section">
    <NavBar></NavBar>
    <b-container class="h-100">
      <b-row align-v="center" align-h="center" class="h-100">
        <b-col cols="10">
          <b-row>
            <b-col>
              <div class="header-content">
                <h1 class="header-heading"
                  >Brando <span class="header-span">suliman</span></h1
                >
                <p class="header-para">web designer and develper</p>
                <Button variant="primary" btnTxt="click me"></Button>
              </div>
              <div class="header-fotter-text">
                <p>follow me</p>
              </div>
            </b-col>
          </b-row>
        </b-col>
      </b-row>
    </b-container>
  </section>
</template>
<script>
import NavBar from "../components/NavBar.vue";
import Button from "../components/Button.vue";
export default {
  components: {
    NavBar,
    Button,
    // Card,
    // Hell
    // oWorld,
  },
};
</script>

<style>
/*HEADER-SECTION*/
#header-section {
  background-image: url(../assets/headrpic.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  height: 100vh;
}
.header-heading {
  color: white;
  font-size: 45px;
  text-transform: capitalize;
  font-weight: bold;
}
.header-span {
  color: #26cb9e;
}
.header-para {
  color: white;
}
/* .header-btn {
  border: none;
  padding: 10px;
  background-color: #3d3d3d;
  color: white;
} */
.header-fotter-text {
  position: absolute;
  /* top: 0; */
  bottom: 0;
  /* left: 0; */
  right: 33px;
  color: white;
}
</style>
