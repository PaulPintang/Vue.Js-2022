<template>
  <FirstComponent person="Paul" />
  <Button color="blue"/>
</template>

<script>
import FirstComponent from "./components/FirstComponent";
import Button from "./components/Button";
export default {
  name: "App",
  props: {
     color: String,
  },
  components: { FirstComponent, Button },
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
