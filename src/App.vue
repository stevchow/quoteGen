<template>
  <div id="app">
    <div class="heading">
      <img src="./assets/logo.png" class="logo" alt="logo">
      <HelloWorld msg="Quote Generator with Progressive Web Apps and Vue.js"/>
    </div>
    <div id="generator">
      <quote-gen></quote-gen>
    </div>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import QuoteGen from "./components/QuoteGen.vue";

let bar;

export default {
  components: {
    HelloWorld,
    QuoteGen
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #ffffff;
}

.logo {
  margin-top: 35vh;
  margin-bottom: -1.5rem;
  width: 60vw;
}

.heading {
  background: #a1ffce; /* fallback for old browsers */
  background: -webkit-linear-gradient(
    to top,
    #faffd1,
    #a1ffce
  ); /* Chrome 10-25, Safari 5.1-6 */
  background: linear-gradient(
    to top,
    #faffd1,
    #a1ffce
  ); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
  height: 100vh;
}

#generator {
  height: 100%;
  background: #ffafbd; /* fallback for old browsers */
  background: -webkit-linear-gradient(
    to top,
    #ffc3a0,
    #ffafbd
  ); /* Chrome 10-25, Safari 5.1-6 */
  background: linear-gradient(
    to top,
    #ffc3a0,
    #ffafbd
  ); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
}
</style>
