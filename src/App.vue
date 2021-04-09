<template>
  <div id="app">
    <Header />
    <BandImage msg="Welcome to Your Vue.js + TypeScript App" />
    <Music />
    <About />
    <Video />
    <Gigs />
    <Footer />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import BandImage from "./components/BandImage.vue";
import Header from "./components/Header.vue";
import Music from "./components/Music.vue";
import About from "./components/About.vue";
import Gigs from "./components/Gigs.vue";
import Footer from "./components/Footer.vue";
import Video from "./components/Video.vue";


@Component({
  components: {
    BandImage,
    Header,
    Music,
    About,
    Gigs,
    Footer,
    Video
  },
})
export default class App extends Vue {}
</script>

<style>
#app {
  font-family: "Roboto Mono", monospace;
  font-style: italic;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
