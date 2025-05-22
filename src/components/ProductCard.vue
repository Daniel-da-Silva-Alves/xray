`<template>
  <div class="product-card">
    <div class="product-img-container">
      <img :src="product.image" class="product-img" :alt="product.name">
    </div>
    <div class="card-body">
      <h5 class="card-title">{{ product.name }}</h5>
      <p class="card-text">{{ product.description }}</p>
      <p class="price">{{ product.price }}</p>
      <button class="btn btn-primary">Adicionar ao carrinho</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ProductCard',
  props: {
    product: {
      type: Object,
      required: true
    }
  }
}
</script>`