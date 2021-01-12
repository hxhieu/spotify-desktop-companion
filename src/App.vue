<template>
  <Toolbar />
  <router-view />
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import Toolbar from './components/Toolbar.vue';

export default defineComponent({
  name: 'App',
  components: {
    Toolbar,
  },
});
</script>

<style lang="scss">
html,
body {
  margin: 0;
  padding: 0;
  overflow: hidden;
}
</style>
