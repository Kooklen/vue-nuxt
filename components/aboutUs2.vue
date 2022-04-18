<template>
  <div>
    <div class="bgi">
      <img src="../assets/AUGZT.webp" alt="">
    </div>
    <div class="main">
      <div class="left">
        <div class="struct">
          构建多元化平台
          用科技创造价值
        </div>
        <div class="really">
          真正的影响力是由人产生的，所以自成立以来，我们崇尚[Amplify your impact], 保持团队的多样性，兼容并包。通过技术增强人类的创造力和提高生产力，用技术改变世界一直是我们的使命。
        </div>
        <div class="AUL1">
          <img src="../assets/AUL1.webp" class="AUL1">
        </div>
        <div class="yiti">
          一站式数字化开发
        </div>
        <div class="we">
          我们不仅为客户提供数字化咨询与开发服务，还自主研发产品&平台，支持创新，培育下一代科技领域的领导者。我们在RPA、HR Tech、AR/VR等领域都有自己的产品推出。
        </div>
        <div class="AUL2">
          <img src="../assets/AUL2.webp" style="width: 586px;">
        </div>
      </div>
      <div class="right">

        <div class="AUR1">
          <img src="../assets/AUR1.webp" alt="">
        </div>

        <div class="FivePlus">
          <div class="first">
            5+全球数字化团队
            持续成长
          </div>
          <div class="second">
            我们相信，不断的学习和分享是成长与创新的捷径。 我们保持奋进，成为提供高质量服务的数字化团队。与此同时，我们[Do what’s
            right]，为自己的行为负责，更为它们对世界的影响负责，我们的数字化行动是为把世界变得更好而努力。
          </div>
        </div>

        <div class="AUR2">
          <img src="../assets/AUR2.webp" alt="">
        </div>
        <div class="mutual">
          <div>
            <div class="first">多样化的产品与平台</div>
            <div class="second">在了解业务背景的基础上，提供的数字化战略咨询服务，利用我们已积累的开发经验，提出针对性解决方案，支持您的业务进行数字化转型。[Create
              value]我们和优秀的客户合作，我们的目标是让企业变得更好。勇于担当，快速行动，始终如一地提供优质服务
            </div>
          </div>
        </div>
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
  //flex-direction: ;
  justify-content: space-between;
  width: 1215px;
  margin: auto;
  margin-top: 118px;
  height: 1170px;
  //background-color: pink;
}

.left {
  //background-color: #0068A0;
  width: 586px;
  height: 1135px;

  .struct {
    width: 287px;
    height: 100px;
    font-size: 36px;
    font-weight: 400;
    color: #000000;
    line-height: 42px;
  }

  .really {
    width: 586px;
    height: 104px;
    font-size: 20px;
    font-weight: 400;
    color: #000000;
    line-height: 23px;
    margin-top: 24px;
  }

  .yiti {
    width: 291px;
    height: 50px;
    font-size: 36px;
    font-weight: 400;
    color: #000000;
    line-height: 42px;
    margin: 30px 0;
  }

  .we {
    width: 503px;
    height: 111px;
    font-size: 20px;
    font-weight: 400;
    color: #000000;
    line-height: 23px;
  }

  .AUL2 {
    margin-top: 48px;
  }

}

.right {
  //background-color: #EEEEEE;
  width: 608px;
  height: 1135px;

  .AUR1 {
    margin: 20px 0 53px 0;
  }

  .FivePlus {
    width: 571px;
    height: 286px;
    margin: 37px 53px 0 37px;
    //background-color: #545454;
    .first {
      width: 302px;
      height: 93px;
      font-size: 36px;
      font-weight: 400;
      color: #000000;
      line-height: 42px;
    }

    .second {
      width: 571px;
      height: 156px;
      font-size: 20px;
      font-weight: 400;
      color: #000000;
      line-height: 23px;
      margin-top: 37px;
    }
  }

  .AUR2 {
    margin: 37px 0 63px 0;
  }

  .mutual {
    width: 571px;
    height: 223px;
    //background-color: skyblue;
    margin: 43px 36px;

    .first {
      width: 324px;
      height: 50px;
      font-size: 36px;
      font-weight: 400;
      color: #000000;
      line-height: 42px;
    }

    .second {
      width: 571px;
      height: 140px;
      font-size: 20px;
      font-weight: 400;
      color: #000000;
      line-height: 23px;
      margin-top: 23px;
    }
  }
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
  margin-top: 280px;
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
    //background: #C4C4C4;
    border-radius: 0px 0px 0px 0px;
    opacity: 1;
    margin-right: 65px;
  }
}
</style>
