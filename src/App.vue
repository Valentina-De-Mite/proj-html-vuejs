<script>
import { state } from "./state.js";
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";

export default {
  name: "App",
  data() {
    return {
      state,
    };
  },

  components: {
    AppHeader,
    AppMain,
  },
};
</script>

<template>
  <body>
    <AppHeader></AppHeader>
    <!-- /header -->

    <AppMain></AppMain>

    <!-- /main -->

    <!-- /footer -->
  </body>
</template>

<style scoped></style>
