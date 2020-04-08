<template>
  <div class="home" v-if="message.length>0">
    <div class="swiper-container aswiper">
      <div class="swiper-wrapper">
        <div class="swiper-slide">
          <img src="../assets/img/demo1.png" alt />
        </div>
        <div class="swiper-slide">
          <img src="../assets/img/demo1.png" alt />
        </div>
        <div class="swiper-slide">
          <img src="../assets/img/demo1.png" alt />
        </div>
      </div>
    </div>
    <!--  -->
    <message />
    <!--  -->
    <msg-detial :msg="message[0]"/>
    <!--  -->
    <other />
    <!--  -->
    <Footer />
  </div>
</template>

<script>
import Swiper from "swiper";
import Message from "../components/Message";
import MsgDetial from "../components/MsgDetial";
import Other from "../components/Other";
import Footer from "../components/Footer";

export default {
  data() {
    return {
      message: ""
    };
  },
  components: {
    Message,
    MsgDetial,
    Other,
    Footer
  },
  created() {
    this.$api.get("data.json", {}, response => {
      if (response.status >= 200 && response.status < 300) {
        this.message = response.data.allData;
      } else {
        alert(response);
        window.location.reload();
      }
    });
    var mySwiper = new Swiper(".aswiper.swiper-container", {
      loop: true
    });
  }
};
</script>
<style>
.swiper-container {
  width: 100%;
  min-height: 212;
  text-align: center;
}
.swiper-container img {
  width: 100%;
}
</style>
