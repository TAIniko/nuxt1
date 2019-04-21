<template lang="html">
  <div id="body">
    <div class="header-container button">
      <!-- topへのリンク -->
      <nuxt-link
        to="/"
        class="menu"
      >
        top
      </nuxt-link>
      <!-- 終了 -->
      <!-- aboutへのリンク -->
      <nuxt-link
        to="/about"
        class="menu"
      >
        about
      </nuxt-link>
      <!-- 終了 -->
      <!-- languageへのリンク -->
      <nuxt-link
        to="/languages"
        class="menu"
      >
        languages
      </nuxt-link>
      <!-- 終了 -->
      <!-- frameworksへのリンク -->
      <nuxt-link
        to="/frameworks"
        class="menu"
      >
        frameworks
      </nuxt-link>
      <!-- 終了 -->
      <!-- worksへのリンク -->
      <nuxt-link
        to="/works"
        class="menu"
      >
        works
      </nuxt-link>
      <!-- 終了 -->
      <!-- contactsへのリンク -->
      <nuxt-link
        to="/contacts"
        class="menu"
      >
        contacts
      </nuxt-link>
    <!-- 終了 -->
    </div>
  </div>
</template>

<script>
export default {
  name:'Myheader'
}

</script>

<style lang="css">
*{
  margin:0;
}
.header-container{
  display: flex;
  justify-content: space-around;
  width:80%;
  margin:auto;
  letter-spacing:3px;
}
.menu{
  width:16%;
  padding:20px;
  text-align:center;
  color:black;
  opacity:0.7;
}


.menu:hover {
  background-color: rgb(230,0,18,0.6);
  transition: 0.4s;
}



</style>
