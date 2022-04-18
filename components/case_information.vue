<template>
  <div>
    <div class="top">
      <div class="first">成功项目和创新研究</div>
      <div class="second">ddl数字化团队在各种行业都有丰富的经验，战略思维结合设计理念及尖端技术，交付影响关键业务成果的解决方案。</div>
    </div>
    <div class="intro">
      <img src="../assets/tree.webp" alt="" class="tree">

      <div class="change">
        <span v-on:mousemove="activeName=1" :class="activeName==1?'highlight':''">
          金融
        </span>
        <span v-on:mousemove="activeName=2" :class="activeName==2?'highlight':''">
          政企
        </span>
        <span v-on:mousemove="activeName=3" :class="activeName==3?'highlight':''">
          医疗
        </span>
        <span v-on:mousemove="activeName=4" :class="activeName==4?'highlight':''">
          零售
        </span>
      </div>

      <div class="case" v-show="activeName=='1'">
        <div>
          <img src="../assets/case1.webp" alt="">
        </div>
        <div>
          <img src="../assets/case2.webp" alt="">

        </div>
        <div>
          <img src="../assets/case3.webp" alt="">

        </div>
        <div>
          <img src="../assets/case4.webp" alt="">

        </div>
      </div>

      <div class="case" v-show="activeName=='2'">
        <div>
          <img src="../assets/case1.webp" alt="">
        </div>
        <div>
          <img src="../assets/case2.webp" alt="">

        </div>
        <div>
          <img src="../assets/case3.webp" alt="">

        </div>
        <div>
          <img src="../assets/case4.webp" alt="">

        </div>
      </div>

      <div class="case" v-show="activeName=='4'">
        <div>
          <img src="../assets/case1.webp" alt="">
        </div>
        <div>
          <img src="../assets/case2.webp" alt="">

        </div>
        <div>
          <img src="../assets/case3.webp" alt="">

        </div>
        <div>
          <img src="../assets/case4.webp" alt="">

        </div>
      </div>

      <div class="case" v-show="activeName=='3'">
        <div>
          <img src="../assets/case1.webp" alt="">
        </div>
        <div>
          <img src="../assets/case2.webp" alt="">

        </div>
        <div>
          <img src="../assets/case3.webp" alt="">

        </div>
        <div>
          <img src="../assets/case4.webp" alt="">

        </div>
      </div>


    </div>
    <FeedBack class="fb"></FeedBack>

  </div>
</template>

<script>
import FeedBack from "@/components/feedBack";

export default {
  name: "case_information",
  components: {FeedBack},
  data() {
    return {
      activeName: '1'
    }
  }
}
</script>


<style scoped lang="less">
.top {
  height: 194px;
  width: 997px;
  margin: auto;

  .first {
    width: 612px;
    height: 88px;
    font-size: 64px;
    font-weight: 400;
    color: #000000;
    line-height: 75px;
  }

  .second {
    width: 997px;
    height: 83px;
    font-size: 24px;
    font-weight: 400;
    color: rgba(0, 0, 0, 0.6);
    line-height: 28px;
    margin-top: 23px;
  }
}

.intro {
  width: 1834px;
  height: 1719px;
  //background: #0068A0;
  border-radius: 0px 0px 0px 0px;
  opacity: 1;
  margin: auto;
  margin-top: 39px;
  position: relative;
}

.tree {
  position: absolute;
  top: 0;
  z-index: 1;
}

.change {
  position: relative;
  z-index: 666;
  width: 260px;
  height: 29px;
  padding: 55px 0 39px 354px;
  color: #FCFCFC;
  font-weight: 400;

  span {
    margin-right: 23px;
    width: 42px;
    height: 29px;
    font-size: 18px;
    line-height: 21px;
  }
}

.case {
  position: relative;
  z-index: 999;
  width: 1126px;
  height: 1285px;
  //background-color: #EEEEEE;
  margin-left: 354px;
  //margin-bottom: 64px;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;

  div {
    margin-right: 25px;
    width: 350px;
    height: 590px;
    background-color: #eee;
  }
}

.fb {
  padding-top: 64px;
  width: 1834px;
  margin: auto;
}

.highlight {
  font-weight: 800;
  //font-size: 48px;
  //color: red;
  //border-bottom: 1px solid #000;
}
</style>
