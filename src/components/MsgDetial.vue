<template>
  <div class="msgDetial">
    <div class="detial">
      <div class="detialLeft">物业类型</div>
      <div class="detialRight">{{msg.type}}</div>
    </div>
    <div class="detial">
      <div class="detialLeft">建筑面积</div>
      <div class="detialRight">{{msg.area}}</div>
    </div>
    <div class="detial">
      <div class="detialLeft">所属楼房</div>
      <div class="detialRight">{{msg.num}}</div>
    </div>
    <div class="detial">
      <div class="detialLeft">所属楼盘</div>
      <div class="detialRight">{{msg.place}}</div>
    </div>
    <!--  -->
    <div>
      <div class="homeType">户型解析</div>
      <div class="describe">
        <img src="../assets/img/demo3.png" alt />
        <span>阔景阳台，美景尽收眼底</span>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  //
  props: {
    msg: Object
  },
  data() {
    return {};
  },
  created() {
  }
};
</script>
<style scoped>
.msgDetial {
  margin: 0 5%;
  font-size: 0.71rem;
  border-bottom: 1px solid #f1f1f1;
  padding-bottom: 10px;
}
.detial {
  display: flex;
  margin-bottom: 1px;
}
.detial .detialLeft {
  flex: 1;
  color: #c6c7ca;
}
.detial .detialRight {
  flex: 4;
}
/*  */
.homeType {
  font-size: 1rem;
  margin: 10px 0;
}
.describe {
  display: flex;
  align-items: center;
}
.describe img {
  width: 20px;
  margin-right: 5px;
}
</style>
