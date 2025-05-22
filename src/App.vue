<!-- App.vue -->
<template>
  <div id="app">
    <Header />
    <Hero />
    <ProductsSection :products="products" />
    <div class="divider"></div>
    <FeaturesSection />
    <CallToAction />
    <Footer />
    <FloatingButton />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import ProductsSection from './components/ProductsSection.vue'
import FeaturesSection from './components/FeaturesSection.vue'
import CallToAction from './components/CallToAction.vue'
import Footer from './components/Footer.vue'
import FloatingButton from './components/FloatingButton.vue'
import { products } from './data/products'

export default {
  name: 'App',
  components: {
    Header,
    Hero,
    ProductsSection,
    FeaturesSection,
    CallToAction,
    Footer,
    FloatingButton
  },
  data() {
    return {
      products
    }
  }
}
</script>

<style>
@import './assets/styles/main.css';
</style>