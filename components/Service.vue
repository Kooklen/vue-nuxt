<template>
  <div>
    <div class="top">
      <div class="mark">
        <img src="../assets/bridge.webp" class="bridge" style="width: 1183px;height: 609px;">

        <div class="flex-col">
          <div class="kong">1</div>

          <div class="marketing">
            数字化精准营销 <br>
            Digital Marketing
          </div>
          <!--              <div>-->
          <!--                使用数据，帮助用户找到最佳匹配促进高效交易。深度挖掘用户生命周期数据化价值，提高营销转化率和风险控制-->
          <!--              </div>-->
          <!--          <div class="usedata"></div>-->
        </div>
      </div>
    </div>

    <div class="experience">
      <div class="first">
        精准聚焦 提投入产出比
      </div>
      <div class="second">
        助您更加了解用户，市场和业务。从线上用户行为到物联网数据，利用数据分析和人工智能，我们帮助你识别和收集信息，通过设计-开发-实施实现业务数据分析，实时发现问题解决问题，最终助力攻克业务难题。
      </div>
    </div>

    <div class="middle">
      <div class="case">
        开发案例
      </div>
      <div class="img">
        <img src="../assets/cd1.webp">
        <img src="../assets/cd2.webp" alt="">
      </div>


    </div>

    <div class="ui">
      <User_image></User_image>
    </div>

    <feed-back class="fb"></feed-back>
  </div>
</template>

<script>
import FeedBack from "@/components/feedBack";
import User_image from "@/components/user_image";

export default {
  name: "service",
  components: {User_image, FeedBack}
}
</script>

<style lang="less" scoped>
.mark {
  margin: auto;
  margin-top: 111px;
  background-color: #0068A0;
  width: 100%;
  height: 497px;
  overflow: visible;
}

.bridge {
  overflow: visible;
  position: absolute;
  top: -2px;
}

.middle {
  width: 1834px;
  height: 657px;
  background: #0068A0;
  border-radius: 0px 0px 0px 0px;
  opacity: 1;
  margin: auto;
  margin-top: 200px;
}

.ui {
  width: 1251px;
  margin: auto;
  margin-top: 200px;
}

.marketing {
  font-size: 48px;
  font-weight: 400;
  color: #FFFFFF;
  line-height: 56px;
  padding: 367px 0 41px 0;
}

.kong {
  width: 1200px;
  height: 495px;
}

.top {
  width: 1834px;
  margin: auto;
}

.experience {
  width: 1142px;
  height: 95px;
  margin: auto;
  margin-top: 73px;
  display: flex;
  flex-direction: row;

  .first {
    width: 226px;
    height: 35px;
    font-size: 24px;
    font-weight: 400;
    color: #53575A;
    line-height: 60px;
  }

  .second {
    margin-left: 117px;
    width: 799px;
    height: 95px;
    font-size: 18px;
    font-weight: 400;
    color: #53575A;
    line-height: 21px;
  }
}


.middle {
  margin-top: 73px;

  .case {
    width: 144px;
    height: 50px;
    font-size: 36px;
    font-weight: 400;
    color: #FFFFFF;
    line-height: 42px;
    padding: 40px 59px;

  }
}

.img {
  display: flex;
  flex-direction: row;
}

.fb {
  margin: auto;
  margin-top: 230px;
  width: 97.5%;
}

.flex-col {
  display: flex;
  flex-direction: row;
}
</style>
