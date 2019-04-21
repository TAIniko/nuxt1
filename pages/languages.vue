<template>
  <div id="language">
    <myheader />
    <title />
    <Title
      class="title"
      :title="languagesTitle"
    />
    <div class="languages-wrapper main">
      <div
        v-for="language in languages"
        :key="language.name"
      >
        <div class="pe">
          <h1>
            {{ language.name }}
          </h1>
          <div class="languageText">
            {{ language.text }}
          </div>
        </div>
        <p>{{ language.level }}</p>
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
      languagesTitle:'languages',
      languages:[
        {
          name:'HTML/CSS',
          text:'Progateを使用して基礎を勉強しました。それ以降は簡単なサイトをまねしながら練習してます。',
          level:'使用歴：１か月'
        },
        {
          name:'Ruby on Rails',
          text:'Progateを使用しtwitterの擬似サイトをつくりました。',
          level:'使用歴：１月か月'
        },
        {
          name:'JavaScript',
          text:'Progateを使用して基礎を勉強しました。',
          level:'使用歴：１か月'
        },
        {
        name:'Ruby',
        text:'Progateを使用して基礎を勉強しました。',
        level:'使用歴：１か月'
      },
      {
        name:'CSS',
        text:'初めて学んだ言語です。大学の授業で基礎はひととうりやりました。関数のグラフの中に打点を打ち面積を求めるプログラムをつくったりしました。',
        level:'使用歴：１か月'
      }
      ]
    }
  },
  layout:'default',
  head(){
    return{
      title:"language"
    }
}
}
</script>
<style>
#language{
  letter-spacing:3px;
}
.languages-wrapper{
  display:flex;
  justify-content:space-around;
  align-content:space-around;
}
.languages-wrapper p{
  font-weight:bold;
}
.languageName{
  font-weight: bold;
}

.pe{
}
</style>
