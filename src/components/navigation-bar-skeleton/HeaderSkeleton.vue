<template>
  <div class="header">
    <div class="logo">Logo</div>
    <div class="header-right">
      <square-icon class="icon"></square-icon>
      <square-icon class="icon"></square-icon>
      <circle-icon class="icon"></circle-icon>
      <rectangle-icon></rectangle-icon>
    </div>
  </div>
</template>

<script>
import SquareIcon from "./SquareIcon";
import RectangleIcon from "./RectangleIcon";
import CircleIcon from "./CircleIcon";
export default {
  components: {
    SquareIcon,
    RectangleIcon,
    CircleIcon,
  },
};
</script>

<style scoped>
.header {
  background-color: #f1f1f1;
  display: flex;
  height: 64px;
  justify-content: space-between;
  align-items: center;
  box-sizing: border-box;
  padding: 0 20px;
}

.header-right {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.header .logo {
  font-size: 25px;
  font-weight: bold;
  color: grey;
  height: 100%;
  display: flex;
  align-items: center;
}

.icon{
    margin: 24px;
}
/* Small phone: from 0 to 480px */
@media only screen and (max-width: 480px) {
  .header-right {
    display: none;
  }
}
</style>