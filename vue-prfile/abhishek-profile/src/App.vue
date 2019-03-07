<template>
  <div id="app">
      <HomePage v-bind:contactMe="contactMe" msg="Hello This is Abhishek" />
  </div>
</template>

<script>
import HomePage from './components/HomePage.vue';
import data from './site-data/data.json';

export default {
  name: 'app',
  components: {
    HomePage
  },
  data() {
    return {
      contactMe:data.contactMe
    }
  },
}

</script>

<style>
body{
  margin:0;
  padding:0;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  display:flex
}

.image_bg{
  background-image: url("./assets/background.jpg");
  background-repeat: no-repeat;
  background-size:cover;
  width:100%;
  height:100vh
}
.image_bg:after{
  background:#000;
  opacity:0.6;
  content:'';
  width:100%;
  height:100%;
  position:absolute
}

.main {
  width:100%;
  height:100%

}
header {
  background-color:#999;
  width:100%;
  margin:0 auto;
}

</style>
