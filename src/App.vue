<script>
import { state } from "./state.js";
import AppHeader from "./components/AppHeader.vue";

export default {
  name: "App",
  data() {
    return {
      state,
    };
  },

  components: {
    AppHeader,
  },
};
</script>

<template>
  <body>
    <AppHeader></AppHeader>
    <!-- /header -->

    <main>
      <div class="jumbotron"></div>
    </main>

    <!-- /main -->

    <!-- /footer -->
  </body>
</template>

<style scoped></style>
