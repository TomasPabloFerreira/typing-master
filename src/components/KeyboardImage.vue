<template>
  <div class="keyboard-image container-fluid">
    <div class="row">
      <div class="col-sm-3"></div>
      <div class="col-sm-6">
        <img id="keyboard-img" src="../../public/images/keyboard.png" />
      </div>
      <div class="col-sm-3"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "KeyboardImage",
  props: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#keyboard-img {
  width: 100%;
}
</style>
