<template>
  <div id="app">
    <AppHeader/>
    <AppMain/>
  </div>
</template>

<script>
import AppHeader from './page/AppHeader.vue';
import AppMain from './page/AppMain.vue';

export default {
  name: 'App',
  components: {
    AppMain,
    AppHeader
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
