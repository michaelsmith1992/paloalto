<template>
  <div class="footer mt-5">
    <a href="#" class="fa fa-facebook icon"></a>
    <a href="#" class="fa fa-twitter icon"></a>
    <a href="#" class="fa fa-instagram icon"></a>
    <a href="#" class="fa fa-spotify icon"></a>
    <a href="#" class="fa fa-apple icon"></a>
    <a href="#" class="fa fa-youtube icon"></a>
    <p>paloaltoband@outlook.com</p>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component
export default class Footer extends Vue {}
</script>

<style>
.footer {
  background-color: rgb(224, 12, 214);
  color: white;
  padding-left: 3rem;
  padding-right: 3rem;
  width: 100%;
  position: absolute;
}

.icon {
  padding: 1.5rem;
}

.footer a {
  color: white;
  text-decoration: none;
    font-size: 3rem
}
.nav-link {
  font-weight: bold;
  color: white;
}

.nav-item {
  color: white;
}

.logo-img {
  height: 5rem;
}

.nav {
  align-self: center;
}
</style>
