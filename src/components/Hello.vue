<template>
  <el-row>
    <el-date-picker :editable="false" v-model="sendTime" type="datetime" placeholder="选择时间范围"></el-date-picker>
  </el-row>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      sendTime: null
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
