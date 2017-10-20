<template>
  <el-row>
    <div>{{msg}}</div>
  </el-row>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: null
    }
  },
  created () {
    this.$ajax.request('/vn').then(res => {
      console.log(res)
      this.msg = res.data
    })
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
