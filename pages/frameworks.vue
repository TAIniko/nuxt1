<template>
  <div>
    <myheader />
    <title />
    <Title
      class="title"
      :title="frameworksTitle"
    />
    <div class="frameworks-wrapper ">
      <div
        v-for="framework in frameworks"
        :key="framework.name"
        class="framework-chil"
      >
        <h1>
          {{ framework.name }}
        </h1>
        <div class="frameworkText">
          {{ framework.text }}
        </div>
        <p>{{ framework.level }}</p>
      </div>
    </div>
    <myfooter />
  </div>
</template>
<script>
import Mtfooter from '@/components/Myfooter'
import Myheader from '~/components/Myheader.vue'
import Title from '~/components/Title.vue'
export default {
  components:{
    Myheader,
    Title,
    Myfooter
  },
  data: function(){
    return{
      frameworksTitle:'frameworks',
      frameworks:[
        {
          name:'Vue.js',
          text:'このポートフォリオサイト作成のために公式ドキュメントをよんで勉強しました。',
          level:'使用歴：1か月'
        },
        {
          name:'Nuxt.js',
          text:'このポートフォリオサイト作成のために公式ドキュメントをよんで勉強しました。',
          level:'使用歴：1か月'
        }
      ]
    }
  },
  layout:'default',
  head(){
    return{
      title:"frameworks"
    }
}
}
</script>
<style>
.frameworks-wrapper{
  display:flex;
  justify-content:space-around;
  align-content:space-around;
  height:500px;
}
.framework-chil{
  margin: 0 20px 40px 0;
  background-color: #f7f7f7;
  border-radius:6px;
  width:30%;
  height:300px;
  padding:20px;
  position:relative;
}
.frameworks-wrapper p{
  font-weight:bold;
  position:absolute;
  bottom:0;
}
</style>
