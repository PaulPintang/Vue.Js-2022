<template lang="">
  <div>
    <h1>{{ person }}</h1>
  </div>
</template>
<script>
export default {
  name: "FirstComponent",
  props: {
    person: String,
  },
};
</script>
<style lang=""></style>
