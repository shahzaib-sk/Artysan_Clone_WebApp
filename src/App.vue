<template>
  <Header />
  <Benefits />
  <Working />
  <Services />
  <Pricing />
  <Customers />
  <FAQ />
  <Action />
  <Footer />
</template>

<script>
import Header from './components/Header.vue'
import Benefits from './components/Benefits.vue';
import Working from './components/Working.vue'
import Services from './components/Services.vue'
import Pricing from './components/Pricing.vue'
import Customers from './components/Customers.vue'
import FAQ from './components/FAQ.vue'
import Action from './components/Action.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: { Header, Benefits, Working, Services, Pricing, Customers, FAQ, Action, Footer }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Lato:ital,wght@0,100;0,300;0,400;0,700;0,900;1,100;1,300;1,400;1,700;1,900&display=swap');
#app {
  font-family: sans-serif, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width: 100%;
  margin: 20px auto;
}
</style>
