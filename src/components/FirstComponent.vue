<template lang="">
  <div>
    <h1>{{ person }}</h1>
    <p>{{ age }}</p>
    <slot></slot>
  </div>
</template>
<script>
export default {
  name: "FirstComponent",
  props: {
    person: String,
    age: Number,
  },
};
</script>
<style lang=""></style>
