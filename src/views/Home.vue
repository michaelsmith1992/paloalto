<template>
  <div class="home">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>

<style>

html, body{
  background-color: black;
}

@media screen and (max-width: 600px) {
  .d-flex {
    display: block !important;
  }
}
</style>
