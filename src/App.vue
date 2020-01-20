<template>
  <div id="app">
    <TopBarComponent />
    <router-view/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import TopBarComponent from '@/components/TopBarComponent.vue';

@Component({
  components: {
    TopBarComponent,
  },
})
export default class App extends Vue {}
</script>

<style lang="less">
#app {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Cantarell, 'Open Sans';
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
