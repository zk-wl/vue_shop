<template>
    <div>
        <el-button typr="info" @click="logout">退出</el-button>
    </div>
    <el-container>
  <el-header>Header</el-header>
  <el-container>
    <el-aside width="200px">Aside</el-aside>
    <el-main>Main</el-main>
  </el-container>
</el-container>
</template>

<script>
export default {
    data () {
        return 
    },
    methods: {
        logout () {
            window.sessionStorage.clear()
            this.$router.push('/login')
        }
    }
}
</script>

<style lang="less" scoped>

</style>