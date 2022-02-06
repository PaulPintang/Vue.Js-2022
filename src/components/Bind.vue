<template>
  <div>
    <a v-bind:href="url">attribute binding</a>
  </div>
</template>

<script>
export default {
  name: "Bind",
  props: {
    url: String,
  },
};
</script>

<style></style>
