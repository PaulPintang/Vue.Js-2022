<template>
  <div>
    <p>Name: {{ name }}</p>
    <p>Age: {{ age }}</p>
    <button @click="changeName">Change Name</button>
  </div>
  <p>Events</p>
  <div class="flex">
    <div @mouseover="handleEvents()" class="box">mouseover</div>
    <div @mouseleave="handleEvents()" class="box">mouseleave</div>
    <div @dblclick="handleEvents()" class="box">doubleclick</div>
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
    handleEvents() {
      console.log("mouse events");
    },
  },
};
</script>

<style scoped>
.flex {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  width: 100%;
  margin-bottom: 10px;
}
.box {
  padding: 40px;
  background: gray;
}
</style>
