<script>
import { state } from "../state";
import cards from "../assets/card.js";
import CardComponent from "../components/CardComponent.vue";

export default {
  name: "AppMain",

  components: {
    CardComponent,
  },
  data() {
    return {
      cards,
    };
  },
};
</script>
<template>
  <main>
    <div class="jumbotron d-flex pt-5">
      <div
        class="container d-flex justify-content-center align-items-center text-center"
      >
        <div class="col-8 h-10">
          <p class="xl cursive">
            Professional Development For Coaches And Leaders
          </p>
          <button class="py-2 px-4 mt-4">Learn More</button>
        </div>
      </div>
    </div>

    <div class="container pt-5 text-center">
      <div class="col-8 m-auto">
        <p class="m fw-bolder">
          Since 2000, weve been partnering with education leaders to
          <span class="m fw-bolder red">increase equity and achivment </span>
          for all students.
        </p>
      </div>
      <div class="cards">
        <div
          class="row row-cols-3 row-cols-md-1 my-5 g-3 grid gap-0 column-gap-3 justify-content-evenly"
        >
          <CardComponent
            v-for="card in cards"
            :image_source="card.image_source"
            :card_title="card.card_title"
            :card_text="card.card_text"
          >
          </CardComponent>
        </div>
      </div>

      <div class="row">
        <div class="col-4 px-5 m-0 d-flex align-items-center">
          <div class="macchia orange col-4 fw-bold fs-1">6500</div>
          <div class="orange fw-bold col-4 fs-1">+</div>
          <div class="fs-4 fw-bold col-4">Students</div>
        </div>
        <div class="col-4 px-5 m-0 d-flex align-items-center">
          <div class="macchia orange col-4 fw-bold fs-1">200</div>
          <div class="orange fw-bold col-2 fs-1">+</div>
          <div class="fs-4 fw-bold col-6">Online Courses</div>
        </div>
        <div class="col-4 px-5 m-0 d-flex align-items-center">
          <div class="macchia orange col-4 fw-bold fs-1">100</div>
          <div class="orange fw-bold col-2 fs-1">%</div>
          <div class="fs-4 fw-bold col-6">Happy Clients</div>
        </div>
      </div>

      <div class="col-8 m-auto mt-5">
        <h2 class="fw-bold">Recent Courses</h2>
        <p class="fs-5 mt-4">
          Whether you're considering a fountation course or an undergraduate
          degree master's or a PhD, academics is a place where students thrive.
        </p>
      </div>
    </div>
  </main>
</template>

<style lang="scss" scoped>
@use "../scss/variables.scss";
.jumbotron {
  background-repeat: no-repeat;
  background-size: cover;
  height: 95vh;
  background-image: url(../assets/img/jumbotron_1.PNG);
}

.main {
  background-color: var(--bgc_primary_1);
}

.xl {
  font-size: 58px;
}

.m {
  font-size: 30px;
}

.macchia {
  background-image: url(../assets/img/counter-shape-1-1-1.png);
  background-repeat: no-repeat;
  background-size: center;
}
.red {
  color: var(--t_red_subtle);
}

.orange {
  color: var(--t_orange);
}
.cursive {
  font-family: "Playfair Display", serif;
}
button {
  background: none;
  border-width: 0.5px;
}
</style>
