<template>
  <div id="app">
    <HelloWorld msg="Welcome to Your Mand Mobile App"/>
    <md-icon name="mand" svg></md-icon>
    <md-icon name="order" svg></md-icon>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue"
import { Icon } from 'mand-mobile'
import './assets/mand.svg'
import './assets/order.svg'

export default {
  name: "app",
  components: {
    HelloWorld,
    [Icon.name]: Icon
  }
};
</script>

<style scoped>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
