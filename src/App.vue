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
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100;400;700&display=swap');

*:focus {
  outline: none !important;
  box-shadow: none;
}

html,
body {
  margin: 0;
  padding: 0;
  overflow: hidden;
  font-family: 'Roboto', sans-serif;
  font-size: 14px;
}
</style>
