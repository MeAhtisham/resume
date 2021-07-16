<template >
<section id="footer">
<b-container>
    <b-row align-v="center">
      <b-col>
        <div class="footer-heading">
          <h2>@2019 copywrite. All reserved</h2>

        </div>
        <div class="icon-img">
          <img src="../assets/facebook.svg" alt="" class="img-fluid">
          <img src="../assets/instagram.svg" alt="" class="img-fluid">
          <img src="../assets/twitter.svg" alt="" class="img-fluid">
          <img src="../assets/home.svg" alt="" class="img-fluid">

        </div>
      </b-col>
    </b-row>
    <div class="my">
      <img src="../assets/up.svg" alt="" class="img-fluid">
    </div>
  </b-container>
</section>
  
</template>

<script>
export default {

}
</script>

<style>
#footer{
  background-color: black;
  padding: 60px 0px;
  position: relative;
}
.footer-heading{
  text-align: center;
}
.footer-heading h2{
  color: white !important;
}
.icon-img{
    margin-top: 15px;
    display: flex;
    justify-content: center;
    align-items: center;
    
}
  .icon-img img{
    width: 20px;
    margin-left: 10px;
    }
    .my
    {
    background-color: white;
    position: absolute;
    top: -20px;
    text-align: center;
    margin: auto;
    right: 0;
    left: 0;
    /* bottom: auto; */
    width: 35px;
    border-radius: 50%;
    height: 35px;
      }
      .my img{

        width: 47%;
       margin-top: 5px;
        }
</style>