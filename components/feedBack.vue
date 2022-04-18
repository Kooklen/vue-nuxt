<template>
  <div>
    <div class="main">
      <div class="word">
        <div class="contactus">联系我们</div>
        <div class="expect">期待收到来自您的信息</div>
      </div>
      <div class="input">
        <div class="small">
          <input type="text" v-model="form.name" placeholder="姓名/Name">
          <input type="text" v-model="form.phone" placeholder="电话/Phone Number">
          <input type="text" v-model="form.company" placeholder="公司/Company">
          <input type="text" v-model="form.email" placeholder="邮箱/Email Address">
          <input type="text" v-model="form.city" placeholder="城市/City">
        </div>
        <div class="message">
          <input type="text" class="messaged" v-model="form.message" placeholder="请留言">
          <button>发送</button>
        </div>
      </div>


    </div>
  </div>
</template>

<script>
export default {
  name: "feedBack",
  data() {
    return {
      form: {
        name: '',
        phone: '',
        company: '',
        email: '',
        city: '',
        message: ''
      }
    }
  }
}
</script>

<style lang="less" scoped>
.main {
  width: 100%;
  height: 1000px;
  background: #343A40;
  //border-radius: 0px 0px 0px 0px;
  //opacity: 1;
}

.contactus {
  width: 286px;
  height: 90px;
  font-size: 48px;
  font-weight: 600;
  color: white;
  line-height: 75px;
  padding: 0;
}

.expect {
  width: 383px;
  height: 55px;
  font-size: 24px;
  font-weight: 600;
  color: white;
  line-height: 42px;
}

.word {
  padding: 80px 0 41px 212px;
}

.input {
  display: flex;
  flex-direction: row;
  margin-left: 212px;
  width: 1000px;
}

.small {
  display: flex;
  flex-direction: column;
  width: 500px;
  height: 472px;
}

.input input {
  color: #EEEEEE;
  font-size: 24px;
  line-height: 28px;
  text-indent: 25px;
  width: 500px;
  //height: 83px;
  background: #606568;
  border: none;
  opacity: 1;
  margin-bottom: 15px;
}

.input .small input {
  height: 83px;
}

.message {
  width: 655px;
  height: 460px;

  button {
    color: white;
    font-size: 24px;
    width: 217px;
    height: 70px;
    background: #C4C4C4;
    border-radius: 0px 0px 0px 0px;
    opacity: 1;
    margin-left: 103px;
  }
}

.messaged {
  width: 655px;
  height: 460px;
  margin-left: 103px;
}


.input input::placeholder {
  color: white;
  text-indent: 25px;
  font-size: 24px;
  line-height: 28px;
}


</style>
