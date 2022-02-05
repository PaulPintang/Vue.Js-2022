<template>
  <FirstComponent person="Paul" />
  <Button color="blue" />
  <Names :names="names" />
</template>

<script>
import FirstComponent from "./components/FirstComponent";
import Button from "./components/Button";
import Names from "./components/Names";
export default {
  name: "App",
  components: { FirstComponent, Button, Names },
  data() {
    return {
      names: [],
    };
  },
  created() {
    this.names = [
      {
        id: 1,
        name: "Paul",
      },
      {
        id: 2,
        name: "John",
      },
      {
        id: 1,
        name: "Mike",
      },
      {
        id: 1,
        name: "Mark",
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
