<template>
  <div class="mt-5" id="about">
    <h2 class="heading">About</h2>
    <div class="container">
      <div class="d-flex mt-5 mob-layout">
        <div class="col-sm">
          <p class="text bio">
            Palo Alto are a 4-Piece Indie Disco band from the bordering city of
            Carlisle. Palo Alto are reviving the indie disco genre fusing huge
            pop hooks, tight grooves and basslines that slap with a psychedelic
            twist. <br /><br />
            Formed not long before the first lockdown Palo Alto have been
            working behind the scenes writing/recording their first set of
            tunes, including debut single “Easy Money” and brand new single "The
            End of the World".
          </p>
        </div>
        <div class="col-sm">
          <img class="band" src="../assets/band2.jpg" />
        </div>
      </div>
      <div class="d-flex mt-5 mob-layout">
        <div class="col-sm">
          <img class="band" src="../assets/band3.jpg" />
        </div>
        <div class="col-sm">
          <h4 class="heading band-members">Band Members</h4>
          <p class="text mt-5">
            Lucia Georgia - Vocals/Keys
          </p>
          <p class="text">
            Michael Smith - Guitar
          </p>
          <p class="text">
            Alexander Whittaker - Bass
          </p>
          <p class="text">
            Nathan Scott - Drums
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component
export default class About extends Vue {}
</script>

<style>
.band {
  max-width: 100%;
  max-height: 100%;
  padding-right: 3rem;
  padding-left: 3rem;
}

.text {
  color: white;
}
.heading {
  color: rgb(224, 12, 214);
  font-weight: bold;
}

@media screen and (max-width: 600px) {
  .band-members {
    margin-top: 3rem;
  }

  .bio {
    margin-bottom: 3rem;
  }
}
</style>
