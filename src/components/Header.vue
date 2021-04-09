<template>
  <div class="header">
    <header class="d-flex flex-wrap justify-content-center py-2 mob">
      <div class="row">
        <div class="col-3"></div>
        <a href="/" class="col-6">
          <img class="logo-img" src="../assets/palologo.png" />
        </a>
        <i class="fa fa-bars col-3 hamburger" v-if="!menu" @click="toggleMenu()"></i>
        <i class="fa fa-times col-3 hamburger" v-if="menu" @click="toggleMenu()"></i>
      </div>

      <ul class="nav nav-pills mob-menu" v-if="menu">
        <li class="nav-item w-100">
          <a @click="scrollTo('#music')" class="nav-link">Music</a>
        </li>
        <li class="nav-item w-100">
          <a @click="scrollTo('#about')" class="nav-link">About</a>
        </li>
        <li class="nav-item w-100">
          <a @click="scrollTo('#video')" class="nav-link">Video</a>
        </li>
        <li class="nav-item w-100">
          <a @click="scrollTo('#gigs')" class="nav-link">Gigs</a>
        </li>
      </ul>
    </header>
    <header class="d-flex flex-wrap justify-content-center py-2 desktop">
      <a
        href="/"
        class="d-flex align-items-center mb-3 mb-md-0 me-md-auto text-dark text-decoration-none logo-link"
      >
        <img class="logo-img" src="../assets/palologo.png" />
      </a>
      <ul class="nav nav-pills">
        <li class="nav-item">
          <a @click="scrollTo('#music')" class="nav-link">Music</a>
        </li>
        <li class="nav-item">
          <a @click="scrollTo('#about')" class="nav-link">About</a>
        </li>
        <li class="nav-item">
          <a @click="scrollTo('#video')" class="nav-link">Video</a>
        </li>
        <li class="nav-item">
          <a @click="scrollTo('#gigs')" class="nav-link">Gigs</a>
        </li>
      </ul>
    </header>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component
export default class Header extends Vue {
  public menu: boolean = false;
  public scrollTo(id: string) {
    const el = document.querySelector(id);
    if (el) {
      const y = el.getBoundingClientRect().top + window.pageYOffset - 140;
      window.scrollTo({ top: y, behavior: "smooth" });
    }
  }
  public toggleMenu() {
    this.menu = !this.menu;
  }
}
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

.mob {
  display: none !important;
}
.desktop {
  display: flex !important;
}

@media screen and (max-width: 600px) {
  .header {
    padding-left: 0;
    padding-right: 0;
  }



  .logo-img {
    height: 3.5rem !important;
    margin-top: 8px;
  }

  .row {
    margin-bottom: 0 !important;
  }

  a.col-6 {
    margin-left: 0 !important;
  }

  .logo-link {
    margin-bottom: 0 !important;
  }
  .mob {
    display: block !important;
  }
  .desktop {
    display: none !important;
  }
  .hamburger {
    align-self: center;
  }
}
</style>
