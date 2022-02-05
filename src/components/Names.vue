<template>
  <div :key="name.id" v-for="name in names">
    <p>{{ name.name }}</p>
  </div>
</template>

<script>
export default {
  name: "Names",
  props: {
    names: Array,
  },
};
</script>

<style></style>
