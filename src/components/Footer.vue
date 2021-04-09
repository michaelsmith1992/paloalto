<template>
  <div class="footer mt-5">
    <a href="https://www.facebook.com/paloaltoband" target="_blank" class="fa fa-facebook icon"></a>
    <a href="https://twitter.com/paloalto_band" target="_blank" class="fa fa-twitter icon"></a>
    <a href="https://www.instagram.com/paloalto_band/" target="_blank" class="fa fa-instagram icon"></a>
    <a href="https://open.spotify.com/artist/15yKJxXGv3Z6qdu6sfkNQC?si=QDNktUxJTX2j9FT63Xnt0A" target="_blank" class="fa fa-spotify icon"></a>
    <a href="https://music.apple.com/ca/artist/palo-alto/1547949966" target="_blank" class="fa fa-apple icon"></a>
    <a href="https://www.youtube.com/channel/UCYLjhfxs21At0ZM3-UWs2RQ" target="_blank" class="fa fa-youtube icon"></a>
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
