<template>
  <div class="main">
    <img src="../assets/band.jpg" class="band-pic" />
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class BandImage extends Vue {
  @Prop() private msg!: string;
}
</script>

<style>
.main {
  padding-top: 5rem;
}

.band-pic {
  width: 100%;
  height: 100%;
}

@media screen and (max-width: 600px) {
  .main {
  padding-top: 5rem;
}
}
</style>
