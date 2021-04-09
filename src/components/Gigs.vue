<template>
  <div class="mt-5 gigs">
    <h2 class="heading">Gigs</h2>
    <div class="container gigs-table mt-5">
      <div class="row table-head">
        <div class="col-sm">
          Date
        </div>
        <div class="col-sm">
          Venue
        </div>
        <div class="col-sm">
          Location
        </div>
        <div class="col-sm">
          Tickets
        </div>
      </div>
      <div class="row gig-info" v-for="gig in gigs" :key="gig.id">
        <div class="col-sm">
          {{ gig.date }}
        </div>
        <div class="col-sm">
          {{ gig.venue }}
        </div>
        <div class="col-sm">
          {{ gig.location }}
        </div>
        <div class="col-sm">
          <a><u>Buy</u></a>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component
export default class Gigs extends Vue {
  data() {
    return {
      gigs: [
        {
          id: 1,
          venue: "The Castle",
          date: "17/12/1992",
          location: "Manchester",
          buyLink: "https://www.seetickets.com",
        },
        {
          id: 1,
          venue: "The Castle",
          date: "18/12/1992",
          location: "Liverpool",
          buyLink: "https://www.seetickets.com",
        },
        {
          id: 1,
          venue: "The Castle",
          date: "19/12/1992",
          location: "London",
          buyLink: "https://www.seetickets.com",
        },
        {
          id: 1,
          venue: "The Castle",
          date: "20/12/1992",
          location: "Bristol",
          buyLink: "https://www.seetickets.com",
        },
        {
          id: 1,
          venue: "The Castle",
          date: "21/12/1992",
          location: "Glasgow",
          buyLink: "https://www.seetickets.com",
        },
      ],
    };
  }
}
</script>

<style>
.cover-art {
  max-width: 100%;
  max-height: 100%;
  padding-top: 3rem;
  padding-right: 3rem;
  padding-bottom: 0.5rem;
  padding-left: 3rem;
}

.table-head {
  font-weight: bold;
  border-bottom: white solid 1px;
  padding-bottom: 1rem;
}

.row {
  margin-bottom: 15px;
}

.gigs-table {
  color: white;
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

@media screen and (max-width: 600px) {
  .table-head {
    display: none;
  }
  .gig-info {
    font-size: x-large;
  }
}
</style>
