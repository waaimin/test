<template>
  <div>
    <div class="footerBlank"></div>
    <div class="footer">
      <div>
        <img src="../assets/img/demo7.png" alt />
        <div>分享</div>
      </div>
      <div>
        <img src="../assets/img/demo8.png" alt />
        <div>关注</div>
      </div>
      <div class="btnOne">
        <div>微聊</div>
        <div>快速在线咨询</div>
      </div>
      <div class="btnTwo">
        <div>电话咨询</div>
        <div>保护你的真实号码</div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  //
};
</script>
<style scoped>
.footerBlank {
  width: 100%;
  height: 10vh;
}
.footer {
  position: fixed;
  width: 100%;
  height: 10vh;
  background: #fff;
  border-top: 1px solid #f1f1f1;
  bottom: 0;
  z-index: 10;
  display: flex;
  font-size: 0.5rem;
  padding: 0 5%;
}
.footer > div {
  width: 12%;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
.footer > div img{
  width: 21px;
  height: 21px;
}
.footer .btnOne {
  width: 33%;
  background: #ff9b15;
  color: #fff;
  border-radius: 5px;
  margin: 2px;
}
.footer .btnTwo {
  width: 33%;
  background: #74c64a;
  color: #fff;
  border-radius: 5px;
  margin: 2px;
}
</style>
