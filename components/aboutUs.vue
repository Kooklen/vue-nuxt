<template>
  <div>
    <div class="bgi">
      <img src="../assets/AUGZT.webp" alt="">
    </div>
    <div class="main">
      <div class="left">
        <div class="construct">
          构建多元化平台
          用科技创造价值
        </div>
        <div class="lLine"></div>
        <div>
          <img src="../assets/AU1.webp" class="AU1">
        </div>
        <div class="wetrust">
          我们相信，不断的学习和分享是成长与创新的捷径。 我们保持奋进，成为提供高质量服务的数字化团队。与此同时，我们[Do what’s
          right]，为自己的行为负责，更为它们对世界的影响负责，我们的数字化行动是为把世界变得更好而努力。
        </div>
        <div class="yiti">
          一站式数字化开发
        </div>
        <div class="Lline2">
        </div>

        <div class="last">
        <span>
          <img src="../assets/AU2.webp" alt="">
        </span>
          <span class="lastword">
          我们不仅为客户提供数字化咨询与开发服务，还自主研发产品&平台，支持创新，培育下一代科技领域的领导者。我们在RPA、HR Tech、AR/VR等领域都有自己的产品推出。
        </span>
        </div>

      </div>
      <div class="right">
        <div>
          <img src="../assets/AU3.webp" alt="">
        </div>
        <div class="influ">
          真正的影响力是由人产生的，所以自成立以来，我们崇尚[Amplify your impact], 保持团队的多样性，兼容并包。通过技术增强人类的创造力和提高生产力，用技术改变世界一直是我们的使命。
        </div>
        <div class="Rline">
        </div>
        <div class="fiveplus">
          5+全球数字化团队
          持续成长
        </div>
        <div class="knowabout">
          <div class="word">
            在了解业务背景的基础上，提供的数字化战略咨询服务，利用我们已积累的开发经验，提出针对性解决方案，支持您的业务进行数字化转型。[Create
            value]我们和优秀的客户合作，我们的目标是让企业变得更好。勇于担当，快速行动，始终如一地提供优质服务
          </div>
          <div>
            <img src="../assets/AU4.webp" alt="">
          </div>
        </div>
        <div class="more">
          多样化的产品与平台
        </div>
        <div class="line6"></div>
      </div>
    </div>
    <div class="team">
      <span>管理团队</span>
    </div>
    <div class="mteam">
      <div></div>
      <div></div>
      <div></div>
      <div></div>
    </div>

  </div>
</template>

<script>
export default {
  name: "aboutUs"
}
</script>

<style scoped lang="less">
.bgi {
  width: 1834px;
  margin: auto;
}

.main {
  display: flex;
  flex-direction: row;
  width: 1560px;
  margin: auto;
  margin-top: 118px;
  height: 1500px;
}

.left {
  width: 744px;
  height: 1154px;
  margin-right: 48px;
  //background-color: #0068A0;
  position: relative;

  .construct {
    width: 448px;
    height: 160px;
    font-size: 46px;
    font-weight: 400;
    color: #000000;
    line-height: 75px;
    margin: 30px 0 0 264px;
    padding: 0;
  }

  .lLine {
    width: 429px;
    height: 0px;
    opacity: 1;
    border: 1px solid #000000;
  }

  .AU1 {
    margin: 121px 0 0 447px;
  }

  .wetrust {
    width: 489px;
    height: 156px;
    font-size: 20px;
    font-weight: 400;
    color: #000000;
    line-height: 23px;
    margin-left: 255px
  }

  .yiti {
    width: 513px;
    height: 80px;
    font-size: 46px;
    font-weight: 400;
    color: #000000;
    line-height: 75px;
    margin: 106px 0 0 231px;
  }

  .Lline2 {
    width: 549px;
    height: 0px;
    opacity: 1;
    border: 1px solid #000000;
  }

  .last {
    width: 718px;
    height: 303px;
    margin: 61px 0 0 26px;
    //background-color: blueviolet;
    display: flex;
    flex-direction: row;
  }

  .lastword {
    width: 489px;
    height: 111px;
    font-size: 20px;
    font-weight: 400;
    color: #000000;
    line-height: 23px;
    padding-top: 194px;
  }
}

.right {
  width: 744px;
  height: 1154px;
  //background-color: #C4C4C4;

  .influ {
    margin: 17px 0 50px 0;
    width: 489px;
    height: 156px;
    font-size: 20px;
    font-weight: 400;
    color: #000000;
    line-height: 23px;
  }

  .Rline {
    width: 400px;
    height: 0px;
    opacity: 1;
    border: 1px solid #000000;
    margin-left: 342px;
  }

  .fiveplus {
    width: 714px;
    height: 235px;
    font-size: 46px;
    font-weight: 400;
    color: #000000;
    line-height: 75px;
  }
}

.knowabout {
  width: 687px;
  height: 255px;
  //background-color: #0068A0;
  display: flex;
  flex-direction: row;

  .word {
    width: 493px;
    height: 111px;
    font-size: 20px;
    font-weight: 400;
    color: #000000;
    line-height: 23px;
    margin-right: 5px;
    margin-top: 153px;
  }
}

.more {
  width: 576px;
  height: 80px;
  font-size: 46px;
  font-weight: 400;
  color: #000000;
  line-height: 75px;
  margin-top: 141px
}

.line6 {
  width: 538px;
  height: 0px;
  opacity: 1;
  border: 1px solid #000000;
  margin-left: 228px;
}

.team {
  width: 225px;
  height: 84px;
  font-size: 55px;
  font-weight: 400;
  color: #000000;
  line-height: 64px;
  margin: auto;
  border-bottom: 1px solid black;
  //margin-top: 301px;
}

.mteam {
  width: 1215px;
  height: 227px;
  display: flex;
  flex-direction: row;
  margin: auto;
  margin-top: 64px;

  div {
    width: 255px;
    height: 227px;
    background: #C4C4C4;
    border-radius: 0px 0px 0px 0px;
    opacity: 1;
    margin-right: 65px;
  }
}
</style>
