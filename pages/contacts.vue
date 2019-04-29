<template>
  <div class="contacts-wrapper">
    <myheader />
    <title />
    <Title
      class="title"
      :title="contactstitle"
    />
    <ul class="main">
      <li><a href="https://twitter.com/yzHM6ssNFiVjMM9">twitter</a></li>
      <li><a href="https://www.facebook.com/takoyaki.simcity.1">facebook</a></li>
      <li><p>mail:taisuke.sum.sub@gmail.com</p></li>
    </ul>
    <myfooter />
  </div>
</template>
<script>
import Myheader from '~/components/Myheader.vue'
import Title from '~/components/Title.vue'
import Myfooter from '@/components/Myfooter'
export default {
  components:{
    Myheader,
    Title,
    Myfooter
  },
  data(){
    return{
      contactstitle:'contacts'
    }
  },
  layout:'default',
  head(){
    return{
      title:"contacts"
    }
}
}
</script>
<style>
.contacts-wrapper{
  letter-spacing:3px;
  text-align:center;
}
li{
  list-style:none;
  color:black;
}
ul{
  background-color:#f7f7f7;
}
</style>
