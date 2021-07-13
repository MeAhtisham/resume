<template>
  <b-container fluid class="theme-navbar">
    <b-row align-v="center" class="inner-container">
      <b-col cols="6">
        <img height="40px" src="../assets/logo.png" alt="" />
      </b-col>
      <b-col cols="6">
        <ul d-flex>
          <li><a href="#">home</a></li>
          <li><a href="#">profile</a></li>
          <li><a href="#">services</a></li>
          <li><a href="#">contactus</a></li>
          <li><a href="#">bog</a></li>
          <li><a href="#">work</a></li>
        </ul>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {};
</script>

<style scoped>
ul {
  list-style-type: none;
  display: flex;
  justify-content: flex-end;
  margin: 0;
  padding: 0;
}

li {
  margin-left: 15px;
}
a {
  text-decoration: none;
  color: white;
}
.theme-navbar {
  border-bottom: 2px solid #2c2c2cbf;
  height: 71px;
  position: absolute;
  top: 0;
}
.inner-container {
  height: 100%;
}
</style>
