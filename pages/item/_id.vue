<template>
  <div>
<!--  (动态路由)接受一个参数（在pages下创建_id表示接受一个url上为id的参数）  -->
    <h2>商品</h2>
    <hr>
    <!-- 判断路由url上是否有id这个参数 -->
    <div v-if="this.$route.params.id">
        商品id:{{this.$route.params.id}}
    </div>
  </div>
</template>

<script>
export default {
  // 设置理由参数的校验规则
  validate ({ params }) {
    // 必须是number类型
    return /^\d+$/.test(params.id)
    // console.log('id的数据类型:', typeof params.id)
  }
}
</script>

<style>

</style>
