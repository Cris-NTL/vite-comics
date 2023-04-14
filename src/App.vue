<script>
import AppHeader from './components/AppHeader.vue';
import AppJumbotron from './components/AppJumbotron.vue';
import AppMain from './components/AppMain.vue';
import AppFeatures from './components/AppFeatures.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  components: {
    AppHeader,
    AppJumbotron,
    AppMain,
    AppFeatures,
    AppFooter,
  },
};
</script>

<template>
  <AppHeader />
  <AppJumbotron />
  <AppMain />
  <AppFeatures />
  <AppFooter />
</template>

<style lang="scss" scoped>
@use "../src/style/general.scss";
</style>