<template>
  <div class="app">
    <header-skeleton></header-skeleton>
    <skeleton-page />
  </div>
</template>

<script>
import HeaderSkeleton from './components/navigation-bar-skeleton/HeaderSkeleton'

import SkeletonPage from "./components/skeleton-components/SkeletonPage";

export default {
  components: {
    SkeletonPage,
    HeaderSkeleton
  },
};
</script>

<style scoped>
.app{
  background-color: #F5F5F5;
}
</style>

