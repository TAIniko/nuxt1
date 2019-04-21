<template lang="html">
  <div class="buttons">
    <a
      class="btn twitter"
      href="https://twitter.com/share?url="
      target="_blank"
      rel="noopener noreferrer"
      aria-label="Share on twitter"
    >
      <span class="link fa fa-twitter" />
    </a>
    <a
      class="btn facebook"
      href="http://www.facebook.com/sharer.php?u="
      rel="noopener noreferrer"
      aria-label="Share on Facebook"
    >
      <span class="link fa fa-facebook" />
    </a>
  </div>
</template>

<script>
export default {
  name:'Myfooter'
}
</script>

<style lang="css" >
.buttons{
  text-align:center;
}
.facebook {
  color: #3b5998;
  font-size:50px;
}
.twitter{
  color: #55acee;
  font-size:50px;
}


.btn{
  display: inline-block;
  width: 80px;
  height: 80px;
  border-radius: 50%;
  background: skyblue;
  text-align:center;
  line-height: 80px;
  }


</style>
