<template>
  <div class="works-wrapper">
    <myheader />
    <title />
    <Title
      class="title"
      :title="workstitle"
    />
    <div class="main">
      <p>{{ content }}</p>
    </div>
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
      workstitle:'works',
      content:'随時追加予定'
    }
  },
  layout:'default',
  head(){
    return{
      title:"works"
    }
}
}
</script>
<style>
.works-wrapper{
  letter-spacing:3px;
}
p{
  text-align:center;
}
</style>
