<template>
  <li @click="handleClick">{{content}}</li>
</template>

<script>
export default {
  props:['content','index'],
  methods:{
    handleClick () {
      // 子组件向父组件通信
      this.$emit('delete',this.index)
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
