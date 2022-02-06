<template>
  <FirstComponent person="Paul" />
  <Button color="gray" />
  <Names :names="names" />
  <Events />
  <Condition />
  <Bind :url="url" />
</template>

<script>
import FirstComponent from "./components/FirstComponent";
import Button from "./components/Button";
import Names from "./components/Names";
import Condition from "./components/Condition";
import Events from "./components/Events";
import Bind from "./components/Bind";
export default {
  name: "App",
  components: { FirstComponent, Button, Names, Events, Condition, Bind },
  data() {
    return {
      url: "https;//impaul.netlify.app",
      names: [],
      name: "name1",
      age: 20,
    };
  },

  created() {
    this.names = [
      {
        id: 1,
        name: "Paul",
        age: 21,
      },
      {
        id: 2,
        name: "John",
        age: 22,
      },
      {
        id: 1,
        name: "Mike",
        age: 24,
      },
      {
        id: 1,
        name: "Mark",
        age: 23,
      },
    ];
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
