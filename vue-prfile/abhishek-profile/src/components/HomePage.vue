<template>

    <div class="home">
      <div class="image_bg">
      </div>
      <h1 class="site_name">{{ msg }}</h1>
      <SocialContacts v-bind:contactMe="contactMe" />
    </div>

</template>

<script>
import SocialContacts from './SocialContacts/SocialContacts.vue';
export default {
  name: 'HomePage',
  props: {
    msg: String,
    contactMe:Array
  },
  components: {
    SocialContacts
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
.home {
  height:100%;
  width:100%;
}
.site_name{
  top:50%;
  transform: translateY(-50%);
  color:#fff;
  font-size:30px;
  text-transform:uppercase;
  color: #fff;
  position: absolute;
  left: 300px;
}

</style>
