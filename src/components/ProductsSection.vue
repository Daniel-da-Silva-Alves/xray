`<template>
  <section id="products" class="products-section">
    <div class="container">
      <h2 class="section-title">Nossos Produtos</h2>
      <div class="row">
        <div class="col-md-4" v-for="(product, index) in products" :key="index">
          <ProductCard :product="product" />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import ProductCard from './ProductCard.vue'

export default {
  name: 'ProductsSection',
  components: {
    ProductCard
  },
  props: {
    products: {
      type: Array,
      required: true
    }
  }
}
</script>`