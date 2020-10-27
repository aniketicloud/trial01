<template>
  <div>
    <div class="line-left"></div>
    <div class="line-right"></div>
  </div>
</template>

<script>
export default {
  components: {
  },
};
</script>

<style>
.line-left {
  height: 25px;
  float: left;
  width: 60%;
  border: 1px solid yellowgreen;
  border-radius: 5px;
  background-color: red;
}

.line-right {
  height: 25px;
  float: right;
  width: 30%;
  border: 1px solid yellowgreen;
  border-radius: 5px;
  background-color: green;
}
</style>