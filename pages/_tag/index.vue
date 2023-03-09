<template>
<!--
  动态路由接受多个参数(创建) :
    1. 创建一个首级参数:文件夹(_tag,index.vue[表示接受第一个参数的路由页面])
      进入页面url路径直接桥对应的tag参数即可如:localhost:3000/ps4 -> 游戏机(ps4)
    2. 在文件夹下创建一个子级文件用于接受第二个参数(_games,用于接受第二个参数)
 -->
  <div>
    <h1>游戏机({{this.$route.params.tag}})</h1>
    <ul>
      <li><a :herf="this.$route.params.tag + '/Zelda'">塞尔达</a></li>
      <li><a :herf="this.$route.params.tag + '/Mario'">马里奥</a></li>
    </ul>
  </div>
</template>
