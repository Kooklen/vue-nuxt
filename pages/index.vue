<template>
  <div>
    <div class="head">
      <el-row>
        <el-col :span="15">
          <div class="logo">
            logo
          </div>
        </el-col>
        <el-col :span="9">
          <el-menu :default-active="activeName" class="el-menu-demo" mode="horizontal" @select="handleSelect">
            <el-menu-item index="first">主页</el-menu-item>
            <el-submenu index="second" @click="this.activeName=second">
              <template slot="title">服务</template>
              <el-menu-item index="second">服务</el-menu-item>
              <el-menu-item index="BigDataApplicationDevelopment">大数据应用开发</el-menu-item>
              <el-menu-item index="DataValueMining">数据价值挖掘</el-menu-item>
              <el-menu-item index="Tapintothevalueofdata">挖掘数据价值</el-menu-item>

            </el-submenu>
            <el-menu-item index="third">案例</el-menu-item>
            <el-menu-item index="fourth">关于我们</el-menu-item>
            <el-menu-item index="fifth">加入我们</el-menu-item>
            <el-menu-item index="sixth">联系我们</el-menu-item>
          </el-menu>
        </el-col>
      </el-row>
    </div>
    <el-tabs v-model="activeName" @tab-click="handleClick">
      <el-tab-pane label="主页" name="first">
        <div class="backgruond">
          <div class="technology-row-top">
            <div class="technology-left">
              <img src="../assets/gzTower.webp" class="gzt">
            </div>
            <div class="technology-right">
              <div class="word-bg">
                <div class="one">挖掘 开发 创新</div>
                <div class="two">
                  <span class="first">“以数为砥、用心成就”</span>
                  <br>
                  <span class="second">是我们的立世使命。</span>
                </div>
                <div class="three">帮助企业深度挖掘数据价值，激活企业的数据灵感，促进企业的数字化发展。我们提供数字化咨询、数据解决方案、数据应用开发等，
                  从业务、用户、企业自身切入，帮助企业数据业务精准落地。
                </div>
              </div>
            </div>
          </div>

          <div class="technology-row-bottom">
            <div class="technology-row-left">
              <div class="first">
                数据价值深度挖掘合作伙伴
              </div>
              <div class="second">
                我们是一家数据咨询与开发公司，我们从客户的业务角度出发，深度开发数据价值，结合专业的数据应用开发，让投入产生切实的业务成果
              </div>
            </div>
            <div class="technology-row-right">
              <img src="../assets/blur.webp" class="blur">
            </div>
          </div>
        </div>
        <div class="middle">
          <span class="sword">成功案例</span>
          <div class="middle-img">
        <span>
          <img src="../assets/Slice3.webp" alt="">
        </span>
            <span>
          <img src="../assets/Slice4.webp" alt="">
        </span>
            <span>
          <img src="../assets/Slice5.webp" alt="">
        </span>
          </div>
        </div>
        <div class="ns">
          <div class="service">
            <div class="our">
              <div class="first">我们的服务</div>
              <div class="second">MORE</div>
            </div>
            <div class="ser">
              <div class="block">
                <span class="first">大数据咨询</span>
                <span class="second"></span>
              </div>
              <div class="block">
                <span class="first">大数据咨询</span>
                <span class="second"> </span>
              </div>
              <div class="block">
                <span class="first">大数据咨询</span>
                <span class="second"> </span>
              </div>
              <div class="block">
                <span class="first">大数据咨询</span>
                <span class="second"> </span>
              </div>
            </div>
          </div>
        </div>
        <div class="contact">
          <feed-back></feed-back>

        </div>
      </el-tab-pane>
      <el-tab-pane label="服务" name="second">
        <service></service>
      </el-tab-pane>
      <el-tab-pane label="案例" name="third">
        <Case_information></Case_information>
      </el-tab-pane>
      <el-tab-pane label="关于我们" name="fourth">
        <!--        <about-us></about-us>-->
        <about-us2></about-us2>
      </el-tab-pane>
      <el-tab-pane label="加入我们" name="fifth">加入我们</el-tab-pane>

      <el-tab-pane label="大数据应用开发" name="BigDataApplicationDevelopment">
        <BigDataApplicationDevelopment></BigDataApplicationDevelopment>
      </el-tab-pane>
      <el-tab-pane label="数据价值挖掘" name="DataValueMining">
        <DataValueMining></DataValueMining>
      </el-tab-pane>
      <el-tab-pane label="挖掘数据价值" name="Tapintothevalueofdata">
        <Tapintothevalueofdata></Tapintothevalueofdata>
      </el-tab-pane>

    </el-tabs>


  </div>
</template>

<script>
import Service from "@/components/Service";
import FeedBack from "@/components/feedBack";
import AboutUs2 from "@/components/aboutUs2";
import BigDataApplicationDevelopment from "@/components/BigDataApplicationDevelopment";
import DataValueMining from "@/components/DataValueMining";
import Tapintothevalueofdata from "@/components/Tapintothevalueofdata";
import Case_information from "@/components/case_information";

export default {
  name: "IndexPage",
  components: {
    Case_information, Tapintothevalueofdata, DataValueMining, BigDataApplicationDevelopment, FeedBack, Service, AboutUs2
  },
  data() {
    return {
      activeName: 'first'
    }
  },
  methods: {
    handleSelect(key, keyPath) {
      this.activeName = key
      console.log(key, keyPath);
    },
    handleClick(tab, event) {
      console.log(tab, event);
    }
  }
}
</script>

<style lang="less" scoped>

.head {
  width: 99%;
  //height: 112px;  //加了就死机
  position: sticky;
  margin: auto;
  background: hsla(0, 0%, 100%, .97);
  top: 0;
  z-index: 9999;
}


/deep/ .el-menu.el-menu--horizontal {
  border: none;
}

/deep/ .el-menu-item {
  font-size: 24px;
}

.el-menu--horizontal > .el-menu-item.is-active {
  border-bottom: 2px solid #0068A0;
  color: #303133;
}

//.el-tabs__nav-wrap .is-top{
//  width: 0;
//  height: 0;
//}

/deep/ .el-submenu__title {
  font-size: 24px;
  //background-color: saddlebrown;
}


.word {
  color: #000;
  margin-top: 40px;
  padding-left: 50px;

  span {
    font-size: 24px;
    color: rgba(0, 0, 0, 0.6);
    width: 81px;
    height: 36px;
    margin-right: 40px;
  }
}


.backgruond {
  margin: auto;
  width: 96%;
  height: 1100px;
  background: #0068A0;
  position: relative;
  margin-top: 100px;
}


.technology-left {
  margin-left: 200px;
  position: relative;
}

.technology-right {
  //position: absolute;
  //right: 100px;
  width: 908px;
  height: 613px;
  padding-left: 400px;
  //background-color: white;
  .word-bg {
    //background-color: white;
    width: 908px;
    //height: 613px;
    margin: 98px 0 0 86px;

    .one {
      width: 545px;
      height: 107px;
      font-size: 48px;
      font-weight: 400;
      color: #FCFCFC;
      line-height: 84px;
      padding-left: 86px;
    }

    .two {
      font-size: 48px;
      padding-left: 60px;
      margin-bottom: 57px;

      .first {
        font-size: 48px;
        line-height: 56px;
        color: #FCFCFC;
      }

      .second {
        padding-left: 80px;
        font-size: 48px;
        line-height: 56px;
        color: #FCFCFC;
      }
    }

    .three {
      width: 508px;
      font-size: 18px;
      color: #FCFCFC;
      font-weight: 400;
      padding-left: 86px;
    }
  }
}


.technology-row-top {
  display: flex;
  flex-direction: row;
  justify-content: center; /* 水平居中 */
}

.technology-row-bottom {
  height: 1200px;
  display: flex;
  flex-direction: row;
  justify-content: center;
  //background: rgba(16, 105, 207, 0.8);
}

.technology-row-left {
  margin: 120px 108px 0 255px;
  //position: absolute;
  //left: 300px;
  //top: 100px;
  .first {
    //width: 450px;
    height: 59px;
    font-size: 32px;
    line-height: 42px;
    color: #FCFCFC;
  }

  .second {

    margin-top: 26px;
    width: 415px;
    font-size: 18px;
    line-height: 42px;
    color: #FCFCFC;
  }
}

.technology-row-right {
  margin: 0;
  padding: 0;
  //transform: scale(1.2);
  //transform-origin: 10cm 10px;
  //width: 870px;
  //height: 620px;
  //background-color: pink;
  //right: 85px;
  //top: 630px;
  //position: absolute;
  //margin-left: 15px;
  //width: 120%;
}

.blur {
  //padding: 3px;
  width: 103.8%;

  //transform: scale(1.7);
  //transform-origin: left 50px -3px;
  //padding-left: 3px;
  //width: 986px;
  //position: absolute;
  //bottom: -100px
}

.gzt {

  position: absolute;
  left: -100px;
  top: -80px;
  //height: 100%;
}


.middle {
  width: 96%;
  height: 635px;
  margin: auto;
  margin-top: 388px;
  background-color: #0068A0;
  //display: flex;
  //flex-direction: row;
  //justify-content: space-between;
  .sword {
    display: block;
    width: 244px;
    height: 59px;
    font-size: 48px;
    font-weight: 600;
    color: #FCFCFC;
    line-height: 56px;
    padding: 82px 0 86px 305px;
  }
}

.middle-img {
  width: 1300px; //原来是1233px
  margin: auto;

  span {
    display: inline-block;
    width: 385px;
    height: 565px;
    background-color: #EEE;
    margin-right: 22px;
  }
}

.ns {
  width: 96%;
  margin: auto;
}

.service {
  margin: auto;
  margin-top: 281px;
  width: 1217px;
  height: 689px;
  //background-color: pink;
  display: flex;
  flex-direction: row;

  .our {
    display: inline-block;
    width: 240px;
    //background-color: grey;
    .first {
      width: 350px;
      height: 67px;
      font-size: 48px;
      font-weight: 400;
      line-height: 56px;
    }

    .second {
      margin-top: 10px;
      font-size: 36px;
    }
  }

  .ser {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    margin-left: 145px;
    //display: inline-block;
    width: 838px;
    height: 689px;

    //background-color: blue;
    .block {
      display: flex;
      flex-direction: row;
      width: 395px;
      height: 325px;

      .first {
        text-indent: 10px;
        //padding: 15px 0 0 34px;
        font-size: 36px;
        width: 250px;
        height: 300px;
        background-color: #EEEEEE;
      }

      .second {
        width: 70px;
        height: 300px;
        background-color: #0068A0;
      }
    }
  }
}

.contact {
  padding: 0;
  margin: auto;
  margin-top: 143px;
  width: 96%;
  height: 1020px;
  background-color: #545454;

  .contactus {
    width: 286px;
    height: 90px;
    font-size: 64px;
    font-weight: 600;
    color: #FFFFFF;
    line-height: 75px;
    padding: 80px 0 99px 212px;
  }

  .nothing {
    width: 1540px;
    height: 472px;
    display: flex;
    flex-direction: row;

    .first {
      width: 500px;
      height: 472px;
      background-color: #0068A0;
      margin-left: 212px;
      margin-right: 103px;
    }

    .second {
      width: 937px;
      height: 472px;
      background-color: blueviolet;
    }
  }
}

</style>
