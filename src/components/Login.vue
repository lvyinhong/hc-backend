<template>
  <div id="app">
    <el-container>
      <el-header>韩创安全部登陆界面</el-header>
      <el-main>
        <div>
          <el-input placeholder="请输入用户名" v-model="username">
            <template slot="prepend">用户名:</template>
          </el-input>
        </div>
        <div>
          <el-input placeholder="请输入密码" v-model="password">
            <template slot="prepend">密   码:</template>
          </el-input>
        </div>
        <div>
          <el-checkbox v-model="checked">记住密码</el-checkbox>
        </div>
        <div>
          <el-button type="primary">登陆</el-button>
          <el-button type="info">注册</el-button>
        </div>
        <div>
          <el-button type="success" icon="el-icon-check" circle title="QQ登陆"></el-button>
          <el-button type="primary" icon="el-icon-edit" circle title="手机登陆"></el-button>
          <el-button type="info" icon="el-icon-message" circle title="邮箱登陆"></el-button>
        </div>
      </el-main>
    </el-container>
  </div>
</template>

<script>
export default {
  name: 'Login',
  data () {
    return {
      username: '',
      password: '',
      checked: ''
    }
  }
}
</script>

<style lang="scss" scoped>
#app {
  border: 0.1rem solid #555555;
  border-radius: 1rem;
  width: 40rem;
  height: 40rem;
  margin: 8rem 85rem;
  section {
    header {
      text-align: center;
      font-size: 2.5rem;
      text-align: center;
      line-height: 6rem;
    }
    .el-main {
      div {
        padding: 1rem 0;
        button {
          margin: 0 2rem 0 6rem;
        }
      }
    }
  }
}
</style>
