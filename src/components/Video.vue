<template>
  <div class="mt-5 video" id="video">
    <h2 class="heading">Video</h2>
    <div class="container">
      <div class="d-flex mt-5 mob-layout">
        <div class="col-sm margin-b2">
          <iframe
            width="560"
            height="315"
            src="https://www.youtube.com/embed/OKuwM-GKGv4"
            title="YouTube video player"
            frameborder="0"
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen
          ></iframe>
        </div>
        <div class="col-sm">
          <iframe
            width="560"
            height="315"
            src="https://www.youtube.com/embed/M891G9UALLU"
            title="YouTube video player"
            frameborder="0"
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen
          ></iframe>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component
export default class Video extends Vue {}
</script>

<style>
.heading {
  color: rgb(224, 12, 214);
  font-weight: bold;
}

@media screen and (max-width: 600px) {
  iframe {
    width: fit-content;
    height: auto;
  }
  .margin-b2 {
        margin-bottom: 2rem;

  }
}
</style>
