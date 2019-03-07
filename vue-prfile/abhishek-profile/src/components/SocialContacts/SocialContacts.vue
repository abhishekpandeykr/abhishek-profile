<template>
    <ul>
        <li class="nav-item" v-for="(item, index) in contactMe" :key="index">
            <a v-bind:href="item.url" v-bind:alt="item" target="blank">
                <img v-bind:src="item.socialImage" v-bind:alt="item" >
            </a>
        </li>
    </ul>
</template>

<script>
export default {
    name:"SocialContacts",
    props:{
        contactMe:Array
    }
}
</script>

<style >
ul {
    position:absolute;
    top:0;
    right:0;
}

.nav-item {
  display:inline-block;
  padding:5px 10px;
  font-size:22px;
  color:#fff
}
.nav-item a{
    color:#fff
}
img {
    width:40px
}
</style>