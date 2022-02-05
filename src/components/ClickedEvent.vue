<template>
  <div>
    <button @click="changeName">Change Name</button>
  </div>
</template>

<script>
export default {
  name: "ClickedEvent",
  methods: {
    changeName() {
      console.log("change name");
    },
  },
};
</script>
