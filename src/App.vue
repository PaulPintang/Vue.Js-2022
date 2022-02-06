<template>
  <FirstComponent person="Paul Justine" age="21">
    <span>This message is slot or template that can pass to a component </span>
    <template v-slot:numbers>
      <ul>
        <li>21</li>
        <li>21</li>
        <li>21</li>
      </ul>
    </template>
  </FirstComponent>
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
        bool: false,
      },
      {
        id: 2,
        name: "John",
        age: 22,
        bool: false,
      },
      {
        id: 3,
        name: "Mike",
        age: 24,
        bool: false,
      },
      {
        id: 4,
        name: "Mark",
        age: 23,
        bool: false,
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
