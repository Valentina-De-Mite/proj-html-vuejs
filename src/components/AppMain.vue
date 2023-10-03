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
          <p class="xl">Professional Development For Coaches And Leaders</p>
          <button class="py-2 px-4 mt-4">Learn More</button>
        </div>
      </div>
    </div>
  </main>
</template>
<style lang="scss" scoped>
.jumbotron {
  background-repeat: no-repeat;
  background-size: cover;
  height: 92vh;
  background-image: url(../assets/img/jumbotron_1.PNG);
}

.xl {
  font-size: 58px;
  font-family: "Playfair Display", serif;
}

button {
  background: none;
  border-width: 0.5px;
}
</style>
