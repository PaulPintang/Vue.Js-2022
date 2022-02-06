<template>
  <div>
    <p>Name: {{ name }}</p>
    <p>Age: {{ age }}</p>
    <button @click="changeName">Change Name</button>
  </div>
</template>

<script>
export default {
  name: "Events",
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
      this.age++;
    },
  },
};
</script>
