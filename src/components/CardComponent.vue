<script>
export default {
  name: "CardComponent",

  props: {
    image_source: String,
    card_title: String,
    card_text: String,
    cod: Number,
  },
  data() {
    return {
      base_src: "../src/assets/",
    };
  },
};
</script>

<template>
  <div
    class="card border p-5 border-top-0 shadow mt-4 d-flex align align-items-center col-3"
  >
    <img
      :src="base_src + image_source"
      class="card-img-top w-25 py-3"
      alt="..."
    />
    <div class="card-body">
      <h4 class="card-title">{{ card_title }}</h4>
      <p class="card-text fs-5">
        {{ card_text }}
      </p>
    </div>
  </div>
</template>

<style lang="scss" scoped></style>
