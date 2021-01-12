<template>
  <div id="toolbar">
    <img v-svg-inline src="../assets/icons/x-circle.svg" />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  components: {},
});
</script>

<style lang="scss" scoped>
@import '../_variables';

#toolbar {
  width: 100%;
  height: 20px;
  background: $mainDark;
  -webkit-app-region: drag;
}
</style>
