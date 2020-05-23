<template>
  <div>
      <lx-header></lx-header>
      <div>{{msg}}</div>
  </div>
</template>
<script>
import LxHeader from './../../components/Header/index'
export default {
  name: 'home',
  data () {
    return {
      msg: '李美婵'
    }
  },
  components: {
    LxHeader
  }
}
</script>
<style lang="less" scoped>
</style>
