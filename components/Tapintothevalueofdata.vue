<template>
  <div>
    <div class="main">
      <div class="blue">
        <div class="bigdata">
          数据咨询 Data Consulting
        </div>
        <div>
          <img src="../assets/office.webp" alt="" class="program">
        </div>
      </div>

      <div class="UX">
        <div class="word">
          <span class="first">提升数据价值： <br>AI驱动，数据分析，效率提升，用户体验优化</span>
          <span class="second">掌控企业数据情况，推动实现切实可行的数据洞察，提供战略、咨询、架构、数据转型和服务</span>
        </div>
      </div>
    </div>

    <div class="case">
      <User_image></User_image>
      <!--    <div class="bar">-->
      <!--      <div class="develop">开发案例</div>-->
      <!--    </div>-->
    </div>

    <div class="fb">
      <feed-back></feed-back>
    </div>
  </div>
</template>

<script>
import FeedBack from "@/components/feedBack";
import User_image from "@/components/user_image";

export default {
  name: "Tapintothevalueofdata",
  components: {User_image, FeedBack}
}
</script>

<style lang="less" scoped>

.main {
  width: 1834px;
  height: 760px;
  margin: auto;

  .blue {
    width: 1834px;
    height: 367.52px;
    background-color: #0068A0;
    position: relative;

    .bigdata {
      width: 428px;
      height: 151px;
      font-size: 48px;
      font-weight: 400;
      color: #FFFFFF;
      line-height: 56px;
      padding: 234px 0 7px 32px;
    }

    .program {
      position: absolute;
      right: 25px;
      top: 0;
    }
  }
}

.UX {
  //height: 152px;
  //width: 1089px;
  margin: auto;
  margin-top: 223px;
  //background-color: #545454;
  .word {
    width: 1089px;
    height: 118px;
    margin: 104px 0 0 142px;
    display: flex;
    flex-direction: row;
    //text-align: center;
    //align-items: center;
    //justify-content: center;

    .first {
      width: 344px;
      height: 101px;
      font-size: 24px;
      font-weight: 600;
      color: #000000;
      line-height: 28px;
      margin-left: 200px;
      margin-right: 54px;
    }

    .second {
      width: 684px;
      height: 102px;
      font-size: 18px;
      font-weight: 400;
      color: #000000;
      line-height: 21px;
    }
  }
}

.case {
  width: 1215px;
  margin: auto;
  margin-top: 100px;
}

.fb {
  margin: auto;
  margin-top: 398px;
  width: 1834px;
}
</style>
