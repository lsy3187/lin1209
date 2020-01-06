<template>
<div>
 <home-header></home-header>
  <home-swiper></home-swiper>
   <home-icons></home-icons>
   <home-recommend></home-recommend>
   <home-weekend></home-weekend>
   </div>
</template>

<script>
import HomeHeader from './components/Header'
import HomeSwiper from './components/Swiper'
import HomeIcons from './components/Icons'
<<<<<<< HEAD
import HomeRecommend from './components/Recommend'
import HomeWeekend from './components/Weekend'
=======
import axios from 'axios'
>>>>>>> index-ajax
export default {
 name:'Home',
 components: {
   HomeHeader,
   HomeSwiper,
<<<<<<< HEAD
   HomeIcons,
   HomeRecommend,
   HomeWeekend
 },
 data (){
  return{
    city:''
  }
 },
=======
   HomeIcons
 },
 methods:{
  getHomeInfo () {
     axios.get('/api/index.json')
      .then(this.getHomeInfoSucc)
  },
  getHomeInfoSucc (res) {
    console.log(res)
 }
},
mounted () {
    this.getHomeInfo()
>>>>>>> index-ajax
 }
</script>

<style>

</style>