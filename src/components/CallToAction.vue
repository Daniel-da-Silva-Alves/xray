<template>
  <section class="cta-section">
    <div class="container">
      <h2 class="cta-title">Pronto para revolucionar seu diagnóstico por imagem?</h2>
      <p class="cta-text">Entre em contato com um de nossos consultores para uma demonstração personalizada dos nossos equipamentos de raio-X e descubra como podemos atender às necessidades específicas da sua clínica ou hospital.</p>
      <button class="btn btn-hero btn-lg" @click="openWhatsapp">Solicitar demonstração</button>
    </div>
  </section>
</template>

<script>
export default {
  name: 'CallToAction',
  methods: {
    openWhatsapp() {
      window.open('https://wa.me/92986143502', '_blank')
    }
  }
}
</script>