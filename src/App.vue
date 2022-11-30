<template>
  <div id="app">
    <AppMain/>
    <AppFooter/>
  </div>
</template>

<script>
import AppFooter from './page/AppFooter.vue';
import AppMain from './page/AppMain.vue';

export default {
  name: 'App',
  components: {
    AppMain,
    AppFooter
}
}
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
