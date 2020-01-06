<template>
<div class="header">
 <div class="header-left">
   <span class="iconfont back-icon">&#xe624;</span>
 </div>
 <div class="header-input">
    <span class="iconfont">&#xe632;</span>
   输入城市/游玩/主题</div>
 <div class="header-right">{{this.city}}
    <span class="iconfont arrow-icon">&#xe64a;</span>
 </div>
</div>
</template>

<script>

export default {
 name:'HomeHeader',
 props:{
   city:String
 }
}
</script>

<style lang="stylus" scoped>
@import '~styles/varibles.styl'
.header
  display :flex
  background:$bgColor
  color :#fff
  line-height :.86rem
.header-left 
  width:.64rem 
  float:left 
  .back-icon
   text-align:center
   font-size:.4rem
.header-input 
  line-height:.64rem
  height:.64rem
  margin-top:.12rem 
  margin-left:.2rem
  height :.64rem
  flex:1
  background:#fff
  border-radius:.1rem
  color:#ccc
  padding-left:.2rem
.header-right 
  width:1.24rem
  float:right
  text-align:center 
  .arrow-icon
   margin-left:-.04rem
   font-size:.24rem
</style>