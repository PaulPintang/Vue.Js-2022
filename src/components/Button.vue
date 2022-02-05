<template>
  <button :style="{ background: color }" @click="onClick()">Button 1</button>
</template>

<script>
export default {
  name: "Button",
  props: {
    color: String,
  },
  methods: {
    onClick() {
      alert("clicked");
    },
  },
};
</script>
