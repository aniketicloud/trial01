<template>
  <div class="container">
    <heading />
    <div style=""></div>
    <two-rows></two-rows>
  </div>
</template>

<script>
import Heading from "./Heading";
import TwoRows from "./TwoRows";

export default {
  components: {
    Heading,
    TwoRows,
  },
};
</script>

<style >
.container{
    padding: 32px;
    height: 566px;
    background-color: yellow;
}
</style>