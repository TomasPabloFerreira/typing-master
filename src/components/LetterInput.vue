<template>
  <span
    class="letter-input bright letterText"
    :class="{
      active: letterData.state == 1,
      fail: letterData.state == 2,
      success: letterData.state == 3,
    }"
  >
    <template v-if="letterData.text == ' '">
      ␣
    </template>
    <template v-else>
      {{ letterData.text }}
    </template>
  </span>
</template>

<script>
export default {
  name: "letter-input",
  props: ["letterData"],
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.letter-input {
  display: inline-flex;
}

.letterText {
  font-size: 3vw;
}

.active {
  background-color: gray;
}
.fail {
  color: red;
}
.success {
  color: green;
}
</style>
