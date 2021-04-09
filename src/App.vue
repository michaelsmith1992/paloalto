<template>
  <div id="app">
    <Header />
    <HelloWorld msg="Welcome to Your Vue.js + TypeScript App" />
    <Music />
    <About />
    <Video />
    <Gigs />
    <Footer />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import HelloWorld from "./components/HelloWorld.vue";
import Header from "./components/Header.vue";
import Music from "./components/Music.vue";
import About from "./components/About.vue";
import Gigs from "./components/Gigs.vue";
import Footer from "./components/Footer.vue";
import Video from "./components/Video.vue";


@Component({
  components: {
    HelloWorld,
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
