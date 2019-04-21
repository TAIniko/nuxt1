<template>
  <div>
    <myheader />
    <title />
    <Title
      class="title"
      :title="frameworksTitle"
    />
    <div class="frameworks-wrapper main">
      <div
        v-for="framework in frameworks"
        :key="framework.name"
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
  </div>
</template>
<script>
import Myheader from '~/components/Myheader.vue'
import Title from '~/components/Title.vue'
export default {
  components:{
    Myheader,
    Title
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
}
.frameworks-wrapper p{
  font-weight:bold;
}
</style>
