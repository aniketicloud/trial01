<template>
  <div class="container">
    <heading/>
    <two-rows></two-rows>
    <spacer />
    <two-rows></two-rows>
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

<style scoped >
.container {
  padding: 32px;
  height: 316px;
  background-color: #FFFFFF;
}

</style>