<template>
  <div class="login">
    <div class="left">
      <h6>欢迎光临</h6>
    </div>
    <div class="right">
      <div class="frame">
        <div class="zhong">
          <h2>欢迎回来</h2>
          <span>----账号密码登录----</span>
          <el-form ref="form" :model="form">
            <el-form-item>
              <el-input
                v-model="form.name"
                placeholder="请输入用户名"
              ></el-input>
            </el-form-item>
            <el-form-item>
              <el-input v-model="form.name" placeholder="请输入密码"></el-input>
            </el-form-item>

            <el-button type="primary">登录</el-button>
          </el-form>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      form: {
        name: ''
      }
    }
  }
}
</script>

<style lang="scss" scoped>
.login {
  height: 100%;
  display: flex;
  align-content: center;
  justify-content: space-between;
  .left {
    width: 67%;
    height: 100%;
    background-color: #6366f1;
    text-align: center;
    h6 {
      font-weight: 700;
      color: white;
      font-size: 3rem;
      line-height: 600px;
    }
  }
  .right {
    width: 33%;
    height: 100%;
    background-color: #fff;
    .frame {
      margin-top: 40%;
      height: 280px;
      //   background-color: #6366f1;
      line-height: 50%;
      .zhong {
        height: 100%;
        display: flex;
        align-items: center;
        justify-content: space-around;
        flex-direction: column;

        h2 {
          font-weight: 700;
          font-size: 1.875rem;
          line-height: 2.25rem;
        }
        span {
          //   background: #a5cd40;
          filter: Alpha(opacity=10);
          -moz-opacity: 0.2;
          opacity: 0.1;
        }
      }
    }
  }
  //   .el-button--primary > span {
  //     display: inline-flex;
  //     align-items: center;
  //   }

  .el-button {
    width: 100%;
    border-radius: 20px;
    height: 15px;
    line-height: 15px !important;
    background-color: #626aef;
  }
}
</style>
