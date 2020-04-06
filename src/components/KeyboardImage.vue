<template>
  <div id="keyboard-image" class="keyboard-image container-fluid">
    <div id="keyboard-image-container" class="row">
      <div class="col-sm-1"></div>
      <div class="col-sm-10">
        <img
          id="keyboard-img"
          class="bg-bright"
          src="../assets/images/keyboard.png"
        />
      </div>
      <div class="col-sm-1"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "keyboard-image",
  props: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#keyboard-image {
  height: 35%;
}

#keyboard-image-container {
  height: 100%;
}

#keyboard-img {
  height: 100%;
  max-width: 100%;
}
</style>
