<template>
  <div id="toolbar">
    <CloseIcon />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import CloseIcon from '../assets/icons/x-circle.svg';

export default defineComponent({
  components: {
    CloseIcon,
  },
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
