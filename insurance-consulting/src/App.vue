<script>
import { store } from './store.js';

import AppHeader from "./components/AppHeader.vue";
/* import AppMain from "./components/AppMain.vue"; */
import AppFooter from "./components/AppFooter.vue";

export default {
  components: {
    AppHeader,
    AppFooter,
  },
};
</script>

<template>
  <div>
    <AppHeader />
    <!-- <AppMain /> -->
    <AppFooter />
  </div>
</template>

<style lang="scss" scoped>
@import 'node_modules/bootstrap/scss/bootstrap';
@import url("https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.3/font/bootstrap-icons.css");

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
</style>
