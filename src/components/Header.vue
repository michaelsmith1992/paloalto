<template>
  <div class="header">
    <header
      class="d-flex flex-wrap justify-content-center py-2"
    >
      <a
        href="/"
        class="d-flex align-items-center mb-3 mb-md-0 me-md-auto text-dark text-decoration-none"
      >
        <img class='logo-img' src='../assets/palologo.png'>
      </a>
      <ul class="nav nav-pills">
        <li class="nav-item"><a href="#" class="nav-link">Music</a></li>
        <li class="nav-item"><a href="#" class="nav-link">About</a></li>
        <li class="nav-item"><a href="#" class="nav-link">Video</a></li>
        <li class="nav-item"><a href="#" class="nav-link">Gigs</a></li>
      </ul>
    </header>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component
export default class Header extends Vue {}
</script>

<style>
.logo {
  font-family: "Mulish", sans-serif;
  color: white;
  font-style: italic;
}
.header {
  background-color: rgb(224, 12, 214);
  color: white;
  padding-left: 3rem;
  padding-right: 3rem;
  position: fixed;
  width: 100%;
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
