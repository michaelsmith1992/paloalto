<template>
  <div class="mt-5 video">
    <h2 class="heading">Video</h2>
    <div class="container">
      <div class="d-flex mt-5">
        <div class="col-sm">
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
</style>
