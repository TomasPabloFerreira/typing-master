<template>
  <div id="app" class="bg-prim">
    <Header></Header>

    <text-input></text-input>

    <keyboard-image></keyboard-image>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import KeyboardImage from "./components/KeyboardImage.vue";
import TextInput from "./components/TextInput.vue";

export default {
  name: "App",
  components: {
    Header,
    TextInput,
    KeyboardImage,
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
  height: 100%;
  overflow: hidden;
}

html,
body {
  height: 100%;
}

.bg-prim {
  background-color: rgb(40, 49, 73);
}
.bg-sec {
  background-color: #404b69;
}
.bg-tert {
  background-color: #00818a;
}
.bg-bright {
  background-color: #dbedf3;
}

.prim {
  color: rgb(40, 49, 73);
}
.sec {
  color: #404b69;
}
.tert {
  color: #00818a;
}
.bright {
  color: #dbedf3;
}

</style>
