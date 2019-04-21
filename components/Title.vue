<template lang="html">
  <div id="title">
    <h1>{{ title }}</h1>
  </div>
</template>

<script>
export default {
  props:{
    title:{
      type:String,
      default: 'Default title'
    }
  }
}
</script>

<style lang="css" scoped>
#title{
  text-align:center;
}
</style>
