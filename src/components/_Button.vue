<template>
  <div class="btn">
    <slot></slot>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'Button',
});
</script>

<style lang="scss">
.btn {
  cursor: pointer;
  -webkit-app-region: no-drag;
}
</style>
