<template>
  <div id="app">
    <app-header></app-header>
    <router-view></router-view>
    <app-footer></app-footer>
  </div>
</template>

<script>
import AppHeader from './views/AppHeader';
import AppFooter from './views/AppFooter';

export default {
  components: {
    AppHeader,
    AppFooter,
  },
}
</script>

<style>
body {
  min-width: 1240px;
}
</style>