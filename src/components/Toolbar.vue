<template>
  <div id="toolbar">
    <label class="title">Hello world</label>
    <Button @click="onClose">
      <img v-svg-inline src="../assets/icons/x-circle.svg" />
    </Button>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

import Button from './_Button.vue';

export default defineComponent({
  components: {
    Button,
  },
  setup() {
    const onClose = () => {
      const { exit } = window._api;
      exit();
    };
    return {
      onClose,
    };
  },
});
</script>

<style lang="scss" scoped>
@import '../_variables';

#toolbar {
  width: 100%;
  /* height: 16px; */
  background: $mainDark;
  -webkit-app-region: drag;
  display: flex;
  align-items: center;
  justify-content: space-between;
  color: #0a4;

  .title {
    margin-left: 4px;
    font-size: 1rem;
  }

  .btn {
    height: 16px;
    width: 16px;
    margin: 2px 4px;
    &:hover {
      color: #fff;
    }

    transition: 0.25s all;
  }
}
</style>
