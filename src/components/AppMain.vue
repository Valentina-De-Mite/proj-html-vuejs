<script>
import { state } from "../state";

export default {
  name: "AppMain",
  data() {
    return {};
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
          <div
            class="card border p-5 border-top-0 shadow mt-4 d-flex align align-items-center"
            style="width: 25rem"
          >
            <img
              src="../assets/svg/svg-0.svg"
              class="card-img-top w-25 py-3"
              alt="..."
            />
            <div class="card-body">
              <h4 class="card-title">Online Coaching</h4>
              <p class="card-text fs-5">
                Lorem ipsum, dolor sit amet consectetur adipisicing elit. Cum
                aut facilis quo quae corrupti nostrum?
              </p>
            </div>
          </div>
          <div
            class="card border p-5 border-top-0 shadow mt-4 d-flex align align-items-center"
            style="width: 25rem"
          >
            <img
              src="../assets/svg/svg-0.svg"
              class="card-img-top w-25 py-3"
              alt="..."
            />
            <div class="card-body">
              <h4 class="card-title">Online Coaching</h4>
              <p class="card-text fs-5">
                Lorem ipsum, dolor sit amet consectetur adipisicing elit. Cum
                aut facilis quo quae corrupti nostrum?
              </p>
            </div>
          </div>
          <div
            class="card border p-5 border-top-0 shadow mt-4 d-flex align align-items-center"
            style="width: 25rem"
          >
            <img
              src="../assets/svg/svg-0.svg"
              class="card-img-top w-25 py-3"
              alt="..."
            />
            <div class="card-body">
              <h4 class="card-title">Online Coaching</h4>
              <p class="card-text fs-5">
                Lorem ipsum, dolor sit amet consectetur adipisicing elit. Cum
                aut facilis quo quae corrupti nostrum?
              </p>
            </div>
          </div>
        </div>
      </div>

      <div class="row d-flex flex-row">
        <div class="col-4 px-5 m-0">
          <div class="macchia orange col-4 fw-bold fs-1">6500</div>
          <div class="orange fw-bold col-4 fs-1">+</div>
          <div class="fs-3 fw-bold col-4">Students</div>
        </div>
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
