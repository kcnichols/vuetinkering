<template>
  <div class="photo-container">
    <img :src="image" v-on:click="counter += 1"/>
  </div>
</template>

<script>
import image from "../assets/logo.png";

export default {
  name : "Photo",
  data () {
    return {
      counter : 0,
      image: image
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
div {
  align-items: center;
  border : 1px solid #ccc;
  display : flex;
  justify-content: center;
  padding : 8px;
}
</style>
