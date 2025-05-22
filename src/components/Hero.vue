<template>
  <section class="hero">
    <div class="container">
      <h1>Soluções Avançadas em Raio-X</h1>
      <p class="lead">Equipamentos de diagnóstico por imagem com a mais alta tecnologia e precisão para profissionais que exigem excelência em seus resultados</p>
      <button class="btn btn-hero btn-lg mt-4" @click="scrollToProducts">Conheça nossos produtos</button>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Hero',
  methods: {
    scrollToProducts() {
      const productsSection = document.getElementById('products')
      if (productsSection) {
        productsSection.scrollIntoView({ behavior: 'smooth' })
      }
    }
  }
}
</script>