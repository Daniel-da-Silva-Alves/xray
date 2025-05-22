<template>
  <div class="container">
    <div class="product-card">
      <div class="product-img-container">
        <img :src="product.image" class="product-img" :alt="product.name" />
      </div>
      <div class="card-body">
        <h5 class="card-title">{{ product.name }}</h5>
        <p class="card-text">{{ product.description }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ProductCard",
  props: {
    product: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style scoped>
.product-card {
  width: 300px; /* tamanho fixo para todos os cards */
  height: 700px; /* tamanho fixo para todos os cards */
  bottom: 7px;
}

.product-img-container {
  width: 100%;
  height: 250px; /* Defina a altura desejada para o container */
  overflow: hidden;
}

.product-img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>
