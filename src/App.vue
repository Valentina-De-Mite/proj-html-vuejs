<script>
import { state } from "./state.js";

export default {
  name: "App",
  data() {
    return {
      state,
    };
  },
};
</script>

<template>
  <body>
    <img class="logo" src="./assets/img/Logo.jpg" alt="" />
    <nav class="navbar navbar-expand navbar-light bg-light">
      <div class="container d-flex justify-content-end">
        <div class="nav navbar-nav">
          <a class="nav-item nav-link active" href="#" aria-current="page"
            >Home</a
          >
          <a class="nav-item nav-link" href="#">About</a>
          <a class="nav-item nav-link" href="#">Academics</a>
          <a class="nav-item nav-link" href="#">Courses</a>
          <a class="nav-item nav-link" href="#">News</a>
        </div>
      </div>
    </nav>

    <!-- /header -->

    <main>
      <div class="jumbotron"></div>
    </main>

    <!-- /main -->

    <!-- /footer -->
  </body>
</template>

<style scoped>
.logo {
  width: 8%;
  position: absolute;
  top: 0;
  left: 20%;
  z-index: 99;
}

body {
  position: relative;
  font-family: "Gabarito", cursive;
}
</style>
