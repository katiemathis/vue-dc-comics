<template>
  <div id="app">
    <HeaderComponent />
    <BodyComponent />
    <FooterComponent />
  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'
import BodyComponent from './components/BodyComponent.vue'
import FooterComponent from './components/FooterComponent.vue'
/*import './assets/js/menuDOM.js'*/


export default {
  name: 'App',
  components: {
    HeaderComponent,
    BodyComponent,
    FooterComponent,
  },


}
</script>

<style>
#app {
  font-family: 'Open Sans', 'Helvetica Neue', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
