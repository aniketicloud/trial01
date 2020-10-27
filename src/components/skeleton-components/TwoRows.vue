<template>
  <div>
    <single-row></single-row>
    <spacer-line></spacer-line>
    <single-row></single-row>
  </div>
</template>

<script>
import SingleRow from "./SingleRow";
import SpacerLine from "./SpacerLine";

export default {
  components: {
    SingleRow,
    SpacerLine,
  },
};
</script>