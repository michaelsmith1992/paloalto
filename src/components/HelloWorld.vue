<template>
  <div class="main">
    <img src="../assets/band.jpg" class="band-pic" />
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class HelloWorld extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

.band-pic {
  width: 100%;
  height: 100%;
}

@media screen and (max-width: 600px) {
  .band-pic {
    margin-top: 8rem;
  }
}
</style>
