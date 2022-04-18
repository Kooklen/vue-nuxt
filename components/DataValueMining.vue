<template>
  <div>
    <div class="main">
      <div class="value">
        数据价值挖掘
        Data Mining
      </div>
      <div class="light">
        <img src="../assets/light.webp" alt="">
      </div>
    </div>
    <div class="word">
      <div class="first">
        全面了解市场,加快业务拓展
      </div>
      <div class="second">
        从塑造差异化的客户体验到扩展您的技术能力，我们的全球足迹为您提供在新市场推出产品的实地知识，包括文化特定的用户行为和技术障碍，全面加速您的事业开拓新的市场。尤其在中国市场，我们提供全面的中国市场本地化服务，从数字化开发到市场营销和商务拓展，我们的成功经验将帮助跨国客户在中国市场获得成功。

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
  name: "DataValueMining",
  components: {User_image, FeedBack}
}
</script>

<style lang="less" scoped>
.main {
  width: 1834px;
  height: 557px;
  background: #0068A0;
  border-radius: 0px 0px 0px 0px;
  opacity: 1;
  margin: auto;
  margin-top: 100px;
  position: relative;

  .value {
    width: 318px;
    height: 131px;
    font-size: 48px;
    font-weight: 400;
    color: #FFFFFF;
    line-height: 56px;
    padding: 409px 0 0 728px;
  }

  .light {
    position: absolute;
    right: 0;
    top: -110px;
  }
}

.word {
  width: 1359px;
  height: 160px;
  margin: auto;
  //background-color: skyblue;
  margin-top: 48px;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;

  .first {
    width: 471px;
    height: 47px;
    font-size: 24px;
    font-weight: 400;
    color: #000000;
    line-height: 28px;
  }

  .second {
    width: 796px;
    height: 90px;
    font-size: 18px;
    font-weight: 400;
    color: #000000;
    line-height: 21px;

  }
}


.fb {
  margin: auto;
  margin-top: 398px;
  width: 1834px;
}

.case {
  background-color: white;
  width: 1215px;
  height: 657px;
  margin: auto;
  margin-top: 100px;
}
</style>
