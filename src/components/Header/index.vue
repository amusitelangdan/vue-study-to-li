<template>
  <div class="header">
      <div @click="handleSelectHeader(item, index)" v-for="(item, index) in headerList" :key="item+index">{{item}}</div>
  </div>
</template>
<script>
export default {
  name: 'LxHeader',
  data () {
    return {
      msg: '头部',
      headerList: ['综合', '用户', '话题', '专栏', 'Live', '严选经典', '电子书']
    }
  },
  methods: {
    handleSelectHeader (item, index) {
      alert(`选择了第${index + 1}个：${item}`)
    }
  }
}
</script>
<style lang="less" scoped>
.header {
    display: flex;
    justify-content: space-between;
    width: 100%;
    padding: 20px;
    background-color: #cccccc;
    box-sizing: border-box;
    div {
        cursor: pointer;
    }
}
</style>
