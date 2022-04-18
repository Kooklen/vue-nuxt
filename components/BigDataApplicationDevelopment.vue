<template>
  <div>
    <div class="main">
      <div class="blue">
        <div class="bigdata">
          大数据应用开发
          Data Applcation Development
        </div>
        <div>
          <img src="../assets/program.png" alt="" class="program">
        </div>
      </div>

      <div class="UX">
        <div class="word">
          <span class="first">用户至上的UX设计</span>
          <span class="second">我们将 "以人为本的设计 "理念引入到项目中，关注人们在日常生活中的行为和体验。用户至上的用户体验设计能自然地融入人们的日常生活，比如通过UX调查&分析，创建角色的服务体验场景，从而创建新的客户旅程地图。</span>
        </div>
      </div>
    </div>
    <div class="case">
      <User_image></User_image>
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
  name: "BigDataApplicationDevelopment",
  components: {User_image, FeedBack}
}
</script>

<style scoped lang="less">
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
      width: 790px;
      height: 127px;
      font-size: 48px;
      font-weight: 400;
      color: #FFFFFF;
      line-height: 56px;
      padding: 234px 0 7px 32px;
    }

    .program {
      position: absolute;
      right: 0;
      top: 0;
    }
  }
}

.UX {
  height: 392px;
  width: 1834px;
  margin: auto;
  //background-color: #545454;
  .word {
    width: 1017px;
    height: 152px;
    margin: 104px 0 0 142px;
    display: flex;
    flex-direction: row;
    //text-align: center;
    align-items: center;
    justify-content: center;

    .first {
      width: 222px;
      height: 34px;
      font-size: 24px;
      font-weight: 600;
      color: #000000;
      line-height: 34px;

    }

    .second {
      width: 724px;
      height: 50px;
      font-size: 18px;
      font-weight: 400;
      color: #000000;
      line-height: 21px;
      margin-left: 91px;
    }
  }
}

.case {
  width: 1215px;
  margin: auto;
  margin-top: 100px;

  .bar {
    width: 100%;
    height: 117px;
    background-color: #0068A0;

    .develop {
      width: 144px;
      height: 50px;
      font-size: 36px;
      font-weight: 400;
      color: #FFFFFF;
      line-height: 42px;
      padding: 40px 0 0 59px;
    }
  }
}

.fb {
  margin: auto;
  margin-top: 398px;
  width: 1834px;
}
</style>
