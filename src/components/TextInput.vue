<template>
  <div id="text-input" class="row">
    <div class="col-sm-1"></div>
    <div id="text-input-container" class="col-sm-10 bg-sec">
    </div>
    <div class="col-sm-1"></div>
  </div>
</template>

<script>
export default {
  name: "TextInput",
  props: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#text-input {
  min-height: 25%;
  margin-top: 5%;
  margin-bottom: 5%;
}

#text-input-container {
  border-radius: 1em;
  border: 1px solid black;
}
</style>
