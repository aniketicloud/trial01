<template>
  <div class="skeleton-page">
    <div class="content-desktop">
      <div class="flex-container">
        <single-sheet class="single-item"></single-sheet>
        <!-- <single-sheet class="single-item"></single-sheet> -->
        <error-component class="single-item"></error-component>
        <single-sheet class="single-item desktop-only"></single-sheet>
      </div>

      <div class="flex-container">
        <single-down-sheet class="single-item"></single-down-sheet>
        <single-down-sheet class="single-item"></single-down-sheet>
        <single-down-sheet class="single-item desktop-only"></single-down-sheet>
      </div>
    </div>

    <div class="content-mobile">
      <div class="flex-container">
        <error-component class="single-item" style="marginBottom:22px"></error-component>
        <single-down-sheet class="single-item" style="marginBottom:22px"></single-down-sheet>
        <single-down-sheet class="single-item" style="marginBottom:22px"></single-down-sheet>
        <single-down-sheet class="single-item" style="marginBottom:22px"></single-down-sheet>
      </div>
    </div>
  </div>
</template>

<script>
import SingleSheet from "./SingleSheet";
import SingleDownSheet from "./SingleDownSheet";
import ErrorComponent from '../error-component/ErrorComponent'
// import Spacer from './Spacer'

export default {
    components: {
    SingleSheet,
    SingleDownSheet,
    ErrorComponent,
    // Spacer
  },
};
</script>

<style scoped>

.skeleton-page{
  padding: 32px;
}

.flex-container {
  padding-bottom: 32px;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-between;
}

.single-item {
  width: 23%;
}

@media only screen and (max-width: 1200px) {
  .content-mobile {
    display: none;
  }
  .content-desktop {
    display: block;
  }
}

/* Big tablets to 1200px (widths smaller than the 1140px row) */
@media only screen and (min-width: 1024px) {
  .content-mobile {
    display: none;
  }
  .content-desktop {
    display: block;
  }
}

/* Small tablets to big tablets: from 768px to 1023px */
@media only screen and (max-width: 1023px) {
  .content-mobile {
    display: none;
  }
  .content-desktop {
    display: block;
  }
}

/* Small phones to small tablets: from 481px to 767px */
@media only screen and (max-width: 767px) {
  .single-item {
    width: 32%;
  }

  .desktop-only {
    display: none;
  }
  .content-mobile {
    display: none;
  }
  .content-desktop {
    display: block;
  }
}

/* Small phone: from 0 to 480px */
@media only screen and (max-width: 480px) {
  .single-item {
    width: 92%;
  }
  .content-desktop {
    display: none;
  }
  .content-mobile {
    display: block;
  }
}
</style>