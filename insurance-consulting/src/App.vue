<script>

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
@use "./style/generals.scss" as *;
@import 'node_modules/bootstrap/scss/bootstrap';
@import url("https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.3/font/bootstrap-icons.css");


</style>
