<template>
  <div>
    <p>Name: {{ name }}</p>
    <button @click="changeName">Change Name</button>
  </div>
</template>

<script>
export default {
  name: "ClickedEvent",
  props: {
    names: Array,
  },
  data() {
    return {
      name: "name1",
      age: 20,
    };
  },
  methods: {
    changeName() {
      //   console.log("change name");
      this.name = "asdsadsa";
    },
  },
};
</script>
