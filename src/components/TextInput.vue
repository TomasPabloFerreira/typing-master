<template>
  <div id="text-input" class="row">
    <div class="col-sm-2"></div>
    <div id="text-input-container" class="col-sm-8 bg-sec">
      <ul id="letterList">
        <li
          v-for="(letterData, index) in lettersData"
          v-bind:key="index"
          class="letter-input-box"
        >
          <letter-input :letterData="letterData"></letter-input>
        </li>
      </ul>
    </div>
    <div class="col-sm-2"></div>
  </div>
</template>

<script>
import LetterInput from "./LetterInput.vue";

export default {
  name: "text-input",
  components: {
    LetterInput,
  },
  props: ["inputString"],
  data: function() {
    return {
      lettersData: [],
    };
  },
  mounted: function() {
    this.mapStringToLettersData();
  },
  methods: {
    mapStringToLettersData: function() {
      this.lettersData = this.inputString
        .split("")
        .map((letter) => ({ text: letter, state: 0 }));
      this.lettersData[0]["state"] = 1;
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#text-input {
  min-height: 25%;
  margin-top: 5%;
  margin-bottom: 5%;
  width: 100%;
}

#text-input-container {
  border-radius: 1em;
  border: 1px solid black;
  width: 100%;
  padding: 1%;
}

#letterList {
  list-style: none;
  display: inline-flex;
  width: 100%;
}

.letter-input-box {
  height: 5%;
  width: 3%;
}
</style>
