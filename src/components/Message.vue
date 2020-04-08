<template>
  <div class="message">
    <div class="titleOne">
      <div class="homeSize">四室两厅两卫-风婉</div>
      <div class="homeState">在售</div>
      <div class="payType">
        <div class="pay">
          <img src="../assets/img/demo2.png" alt />
          <div>算月供</div>
        </div>
      </div>
    </div>
    <!--  -->
    <div class="titleTwo">
      <div class="priceAll">
        <span>总价约</span>
        <span class="price">104</span>
        <span>万元</span>
      </div>
      <div class="priceOne">单价约8000元/m&sup2;</div>
    </div>
    <!--  -->
    <div class="titleThree">
      <div>大面积阳台</div>
      <div>U型厨房</div>
      <div>观景飘窗</div>
      <div>户型方正</div>
    </div>
  </div>
</template>
<script>
export default {
  //
};
</script>
<style scope>
.message {
  padding: 10px 5%;
  font-size: 1rem;
}
.titleOne {
  display: flex;
  align-items: center;
}
.titleOne .homeSize {
  flex: 4;
  font-weight: bold;
}
.titleOne .homeState {
  flex: 1;
  background: #fb7a7e;
  color: #fff;
  text-align: center;
  font-size: 0.5rem;
}
.titleOne .payType {
  flex: 2;
  display: flex;
  flex-direction: column;
  align-items: flex-end;
  font-size: 0.5rem;
  color: #b1c4d2;
}
.titleOne .payType .pay{
  display: flex;
  flex-direction: column;
  align-items: center;
}
.titleOne .payType img {
  width: 15px;
  height: 15px;
}
/*  */
.titleTwo{
  display: flex;
  align-items: center;
  justify-content: flex-start;
  font-size: 0.5rem;
}
.titleTwo .priceAll{
  display: flex;
  align-items: center;
  color: red;
  margin-right: 5px;
}
.titleTwo .priceAll .price{
  font-size: 1rem;
}
.titleTwo .priceOne{
  color: #bebdc3;
}
.titleThree{
  width: 100%;
  padding-bottom: 10px;
  margin-top: 10px;
  border-bottom: 1px solid #f1f1f1;
  display: flex;
  font-size: 0.3rem;
}
.titleThree div{
  background: #18c897;
  padding: 2px;
  margin-right: 2px;
  color: #fff;
}
.titleThree div:nth-child(2){
  background: #e0a0a1;
}
.titleThree div:nth-child(3){
  background: #edc898;
}
.titleThree div:nth-child(4){
  background: #c5aadd;
}
</style>
