<template>
  <div>
    <div class="container">
      <div class="wrap">
        <nuxt-link to="#">
          <div class="triangle1" />
          <div class="text1">
            top
          </div>
        </nuxt-link>
      </div>

      <div class="wrap">
        <nuxt-link to="/about">
          <div class="triangle2" />
          <div class="text2">
            about
          </div>
        </nuxt-link>
      </div>

      <div class="wrap">
        <nuxt-link to="/languages">
          <div class="triangle1" />
          <div class="text1">
            languages
          </div>
        </nuxt-link>
      </div>

      <div class="wrap">
        <nuxt-link to="frameworks">
          <div class="triangle2" />
          <div class="text2">
            frameworks
          </div>
        </nuxt-link>
      </div>

      <div class="wrap">
        <nuxt-link to="works">
          <div class="triangle1" />
          <div class="text1">
            works
          </div>
        </nuxt-link>
      </div>

      <div class="wrap">
        <nuxt-link to="contacts">
          <div class="triangle2" />
          <div class="text2">
            contacts
          </div>
        </nuxt-link>
      </div>
    </div>
  </div>
</template>

<script>
export default{
}
</script>

<style>
@import url('https://maxcdn.bootstrapcdn.com/font-awesome/4.3.0/css/font-awesome.min.css');
.container{
  display:flex;
  width:100%;
  justify-content: center;
  position: absolute;
	top: 50%;
	left: 50%;
	transform: translate(-50%, -50%);
}

.wrap {
  -webkit-transform: translateY(-500%);
  -ms-transform: translateY(-500%);
  transform: translateY(-500%);
}

/*三角形１*/
.triangle1{
  border-top: 86.6025px solid rgb(255,0,81,0.6);
  border-right: 50px solid transparent;
  border-left: 50px solid transparent;
  display: block;
  transition-duration: 0.3s;
  margin:5px;
}

/*hover時アニメーション*/
a:hover .triangle1{
  transform: scale(1.2);
  transition-duration: 0.3s;
  display: block;
}

/*三角形２*/
.triangle2{
  border-right: 50px solid transparent;
  border-bottom: 86.6025px solid rgb(159, 242, 173,0.7);
  border-left: 50px solid transparent;
  margin:5px;
}

/*hover時アニメーション*/
a:hover .triangle2{
  transform: scale(1.2);
  transition-duration: 0.3s;
}

/*三角形の中に表示する文字*/
.text1 {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  margin: auto;
  text-align: center;
  display: none;
  height:80%;
  color:black;
  opacity: 0.7;
  font-size:20px;
}

.text2{
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  margin: auto;
  text-align: center;
  display: none;
  height:0%;
  color:black;
  opacity: 0.7;
  font-size: 20px;
}

/*textに対するhoverアニメーション*/
a:hover .triangle1 ~ .text1,a:hover .triangle2 ~ .text1{
display:block;
transition:0.3s;
}

a:hover .triangle1 ~ .text2,a:hover .triangle2 ~ .text2{
display:block;
transition:0.3s;
}

/*アニメーション設定*/
.wrap:nth-child(1) {
  -webkit-animation: example 1.0s ease 0.2s 1 forwards;
  animation: example 1.0s ease 0.2s 1 forwards; }

.wrap:nth-child(2) {
  -webkit-animation: example 1.0s ease 0.5s 1 forwards;
  animation: example 1.0s ease 0.5s 1 forwards; }

.wrap:nth-child(3) {
  -webkit-animation: example 1.0s ease 0.2s 1 forwards;
  animation: example 1.0s ease 0.2s 1 forwards; }

.wrap:nth-child(4) {
  -webkit-animation: example 1.0s ease 0.5s 1 forwards;
  animation: example 1.0s ease 0.5s 1 forwards; }

.wrap:nth-child(5) {
  -webkit-animation: example 1.0s ease 0.2s 1 forwards;
  animation: example 1.0s ease 0.2s 1 forwards; }

.wrap:nth-child(6) {
  -webkit-animation: example 1.0s ease 0.5s 1 forwards;
  animation: example 1.0s ease 0.5s 1 forwards; }

@-webkit-keyframes example {
  100% {
    opacity: 1;
    -webkit-transform: translateY(0);
    -ms-transform: translateY(0);
    transform: translateY(0); } }
@keyframes example {
  100% {
    opacity: 1;
    -webkit-transform: translateY(0);
    -ms-transform: translateY(0);
    transform: translateY(0); }
  }


</style>
