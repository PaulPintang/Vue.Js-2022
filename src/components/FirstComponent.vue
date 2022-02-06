<template lang="">
  <div>
    <h1>{{ person }}</h1>
    <slot name="numbers"></slot>
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
