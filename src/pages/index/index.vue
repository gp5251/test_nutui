<template>
  <view class="index">
  <nut-tabs v-model="state.tab1value">
    <nut-tabpane title="Tab 1">
      Tab 1
    </nut-tabpane>
    <nut-tabpane title="Tab 2">
      Tab 2
    </nut-tabpane>
    <nut-tabpane title="Tab 3">
      Tab 3
    </nut-tabpane>
  </nut-tabs>
  </view>
</template>

<script lang="ts">
import {reactive } from "vue";
export default {
  name: "Index",
  components: {},
  setup() {
    const state = reactive({
      tab1value: '0',
    });

    // setTimeout(() => {
    //   state.tab1value = '2';
    // }, 3000);

    return {
      state
    }
  },
};
</script>

<style lang="scss">
.index {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  height: 100%;
  width: 100%;
  overflow: hidden;
}
</style>
