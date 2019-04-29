<template lang="html">
  <div class="buttons">
    <a
      class="btn-tw twitter"
      href="https://twitter.com/share?url="
      target="_blank"
      rel="noopener noreferrer"
      aria-label="Share on twitter"
    >
      <span class="link fa fa-twitter" />
    </a>
    <a
      class="btn-fa facebook"
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
  margin-top:50px;
}
.facebook {
  color: #3b5998;
  font-size:50px;
}
.twitter{
  color: #55acee;
  font-size:50px;
}
.fa{
  /* transform:rotate(45deg); */
}


.btn-tw{
  margin-right:50px;
  display: inline-block;
  width: 80px;
  height: 80px;
  border-radius: 50%;
  text-align:center;
  line-height: 80px;
}
.btn-fa{
  display: inline-block;
  width: 80px;
  height: 80px;
  border-radius: 50%;
  text-align:center;
  line-height: 80px;
}
.twitter:hover{
  color:white;
}
.facebook:hover{
  color:white;
}
.btn-tw:hover{
  background-color:#55acee;
}
.btn-fa:hover{
  background-color:#3b5998;
}


</style>
