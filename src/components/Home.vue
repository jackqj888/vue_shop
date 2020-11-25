<template>
    <div>
        <el-button type="info" @click="logout">退出</el-button>
    </div>
</template>

<script>
export default {
  methods: {
    logout () {
      window.sessionStorage.clear() // 清空 token
      this.$router.push('/login') // 跳转 login
    }
  }

}
</script>

<style lang="less" scoped>

</style>
