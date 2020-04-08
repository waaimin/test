<template>
  <div class="other">
    <div class="title">
      <div>本楼盘其他户型</div>
      <div>
        <div class="type">
          <span class="more">更多户型</span>
          <img src="../assets/img/demo6.png" alt />
        </div>
      </div>
    </div>
    <!--  -->
    <div>
      <div class="swiper-container bswiper">
        <div class="swiper-wrapper">
          <div class="swiper-slide">
            <img src="../assets/img/demo4.png" alt />
            <div class="homeType">3室2厅2卫-110m&sup2;</div>
            <div class="homeState">
              <div>在售</div>
              <div>明明厨卫</div>
              <div>户型方正</div>
            </div>
          </div>
          <div class="swiper-slide">
            <img src="../assets/img/demo5.png" alt />
            <div class="homeType">3室2厅2卫-110m&sup2;</div>
            <div class="homeState">
              <div>在售</div>
              <div>明明厨卫</div>
              <div>户型方正</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import Swiper from "swiper";
export default {
  mounted() {
    var mySwiper = new Swiper(".bswiper.swiper-container", {
      loop: true,
      slidesPerView:2,
      spaceBetween:10
    });
  },
};
</script>
<style scoped>
.other {
  margin: 10px 5%;
  font-size: 1rem;
}
.title {
  display: flex;
  justify-content: space-between;
  margin-bottom: 10px;
}
.title .type {
  display: flex;
  align-items: center;
}
.title .type .more {
  margin-right: 5px;
  font-size: 0.7rem;
  color: #a8aeb3;
}
.bswiper{
  text-align: left;
}
.bswiper .homeType{
  font-size: 0.5rem;
}
.bswiper .homeState{
  display: flex;
  font-size: 0.25rem;
  margin-top: 3px;
}
.bswiper .homeState div{
  background: #f97c75;
  color: #fff;
  margin-right: 2px;
  padding: 1px;
}
.bswiper .homeState div:nth-child(2){
  background: #fef3e8;
  color: #fcc586;
}
.bswiper .homeState div:nth-child(3){
  background: #f5f2f9;
  color: #c9afe0;
}
.bswiper img{
  border: 1px solid #f1f1f1;
}
</style>
