<template>
  <div class="container">
    <div class="upper-skeleton">
      <heading />
      <two-rows></two-rows>
      <spacer />
      <two-rows></two-rows>
      <spacer />
      <two-rows></two-rows>
      <spacer />
      <two-rows></two-rows>
    </div>
  </div>
</template>

<script>
import Heading from "./Heading";
import TwoRows from "./TwoRows";
import Spacer from "./Spacer";

export default {
  components: {
    Heading,
    TwoRows,
    Spacer,
  },
};
</script>

<style scoped>
.container {
  padding: 32px;
  background-color: #ffffff;
  height: 566px;
}
</style>>
