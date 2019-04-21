<template>
  <div id="about">
    <myheader />
    <title />
    <Title
      class="title"
      :title="abouttitle"
    />
    <div class="about-wrapper main">
      <tr
        v-for="(contact, index) in objects"
        :key="index"
      >
        <th>
          {{ contact.key }}
        </th>
        <div class="about-text">
          {{ contact.value }}
        </div>
      </tr>
    </div>
    <myfooter />
  </div>
</template>
<script>
  import Myheader from '~/components/Myheader.vue'
  import Myfooter from '@/components/Myfooter'
  import Title from '~/components/Title.vue'
  export default {
   components:{
      Myheader,
      Myfooter,
      Title
       },
    data(){
      return{
        abouttitle:'about',
        objects: [
        { key: 'name', value: '住ノ井　太佑(21)'},
        { key: 'birthday', value: '1998/01/06'},
        {
          key:'自己紹介', value:'猫が好きです。新しい技術への順応性が高く常に好奇心と探求心を忘れないようなフロントエンジニアを目指して勉強中です。'
        }
      ]
      }
    },
    layout:'default',
       head(){
    return{
      title:"about"
         }
        }
        }
</script>
<style>

#about{
  letter-spacing:3px;
}
.about-wrapper{

}
th{
  padding-right:30px;
  padding-top:15px;
}
tr{
  flex-wrap:wrap;
}
.about-text{
  display:block;
}
</style>
