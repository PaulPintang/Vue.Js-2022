<template>
  <div>
    <div v-if="showName">
      {{ name }}
    </div>
    <button @click="showMyName">
      <span v-if="showName">Hide Name</span>
      <span v-if="!showName">Show Name</span>
    </button>
  </div>
</template>

<script>
export default {
  name: "Condition",
  data() {
    return {
      showName: true,
      name: "Paul Justine Pintang",
    };
  },
  methods: {
    showMyName() {
      this.showName = !this.showName;
    },
  },
};
</script>

<style></style>
