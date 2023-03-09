<template>
  <div>
    <h1>游戏名称222{{this.$route.params.tag}}</h1>
    <h1>游戏名称111{{this.$route.params.tag}}</h1>
    <h1>游戏名称333{{this.$route.params.tag}}</h1>
    <h1>游戏名称aaa{{this.$route.params.tag}}</h1>
    <h1>游戏名称444{{this.$route.params.tag}}</h1>
    <h1>游戏名称555{{this.$route.params.tag}}</h1>
    <h1>游戏名称666{{this.$route.params.tag}}</h1>
    <h1>游戏名称777{{this.$route.params.tag}}</h1>
    <h1>游戏名称888{{this.$route.params.tag}}</h1>
    <h1>游戏名称999{{this.$route.params.tag}}</h1>
    <h1>游戏名称bbb{{this.$route.params.tag}}</h1>
    <hr>
<!--  设置动态路由的二级参数:
      在一级路由参数的文件夹下(_tag)多设置另一个以`_参数`名命名的.vue文件
      此时路由url上面的页面跳转就会重一级路由文件夹继续向下寻找: `_参数`
      结尾的.vue文件,同时当路由url上有对应的参数时就渲染该文件!
  -->
    <div v-if="this.$route.params.Gname">
<!--   此时路由url: ...../tag/Gname ==> /ps4/Zelda(例如)  -->
      游戏 :{{this.$route.params.tag}} - {{this.$route.params.Gname}}
    </div>
  </div>
</template>
