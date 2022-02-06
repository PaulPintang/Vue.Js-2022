<template>
  <div :key="name.id" v-for="name in names">
    <p @click="handleClick(name)" :class="{ underline: name.bool }">
      {{ name.name }}
      {{ name.bool }}
    </p>
  </div>
</template>

<script>
export default {
  name: "Names",
  props: {
    names: Array,
  },
  methods: {
    handleClick(name) {
      name.bool = !name.bool;
    },
  },
};
</script>

<style>
.underline {
  text-decoration: line-through;
}
</style>
