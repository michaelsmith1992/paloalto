<template>
  <div class="mt-5 music" id="music">
    <h2 class="heading">Music</h2>
    <div class="container">
      <div class="d-flex mob-layout">
        <div class="col-sm">
          <img class="cover-art" src="../assets/eotw-ida.jpg" />
          <div class="music-btn"><a href="https://open.spotify.com/track/4ALvpri5PHp7KorgV62Dfm?si=59cb2c56cacb429a">Stream</a></div>
          <div class="music-btn"><a href="https://www.youtube.com/watch?v=OKuwM-GKGv4">Watch Video</a></div>
        </div>
        <div class="col-sm">
          <img class="cover-art" src="../assets/easy-money-cover-2.jpg" />
          <div class="music-btn"><a href="https://open.spotify.com/track/4ALvpri5PHp7KorgV62Dfm?si=59cb2c56cacb429a">Stream</a></div>
          <div class="music-btn"><a href="https://www.youtube.com/watch?v=M891G9UALLU">Watch Video</a></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component
export default class Music extends Vue {}
</script>

<style>
.cover-art {
  width: 100%;
padding-top: 3rem;
    padding-right: 3rem;
    padding-bottom: 0.5rem;
    padding-left: 3rem;
}

.heading {
  color: rgb(224, 12, 214);
  font-weight: bold;
}

.music-btn {
  color: white;
  background-color: rgb(224, 12, 214);
  border: white solid 6px;
  padding: 6px;
  font-weight: bold;
  max-width: 100%;
  margin-left: 3rem;
  margin-right: 3rem;
  margin-top: 10px;
  height: 3rem;
  align-self: center;
}
</style>
