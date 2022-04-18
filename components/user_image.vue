<template>
  <div class="user_main">
    <div class="block">
      <span>用户画像</span>
      <div class="arrow_bg">
        <img src="../assets/arrow_right.svg" class="arrow"></div>
    </div>
    <div class="block">
      <span>数据建模</span>
      <div class="arrow_bg">
        <img src="../assets/arrow_right.svg" class="arrow"></div>
    </div>
    <div class="block">
      <span>个性服务</span>
      <div class="arrow_bg">
        <img src="../assets/arrow_right.svg" class="arrow"></div>

    </div>
    <div class="block">
      <span>营销业务决策</span>
      <div class="arrow_bg">
        <img src="../assets/arrow_right.svg" class="arrow"></div>
    </div>
    <div class="block">
      <span>营销业务落地</span>
      <div class="arrow_bg">
        <img src="../assets/arrow_right.svg" class="arrow"></div>

    </div>
  </div>
</template>

<script>
export default {
  name: "user_image"
}
</script>

<style lang="less" scoped>
.user_main {
  display: flex;
  //flex-direction: column;
  flex-wrap: wrap;
  width: 1215px;
  height: 700px;
}

.block {
  display: flex;
  justify-content: space-between;
  width: 546px;
  height: 75px;
  //background-color: pink;
  border-bottom: 1px solid #333333;
  margin-right: 57px;

  span {
    font-size: 24px;
    color: #333333;
    height: 75px;
    line-height: 75px;
  }
}

.arrow_bg {
  background-color: #00669e;
}

.arrow {
  width: 50px;
  height: 75px;
  margin: auto;
  color: white;
}

</style>
