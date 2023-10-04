<script>
import { state } from "../state";
import variables from "../scss/variables.scss";
export default {
  name: "AppHeader",

  data() {
    return {};
  },
};
</script>

<template>
  <body>
    <img class="logo" src="../assets/img/Logo.jpg" alt="" />
    <nav class="navbar navbar-expand navbar-light bg-light py-3">
      <div class="container d-flex justify-content-end">
        <div class="nav navbar-nav fs-5">
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
  </body>
</template>

<style lang="scss" scoped>
.logo {
  width: 8%;
  position: absolute;
  top: 0;
  left: 20%;
  z-index: 99;
}

.navbar {
  position: relative;
  font-family: "Gabarito", cursive;
}
</style>
