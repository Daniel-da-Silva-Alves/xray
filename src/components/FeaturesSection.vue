`<template>
  <section id="features" class="features-section">
    <div class="container">
      <h2 class="section-title">Por que escolher a X-Ray Solutions?</h2>
      <div class="row">
        <div class="col-md-4 mb-4" v-for="feature in features" :key="feature.title">
          <FeatureCard v-bind="feature" />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import FeatureCard from './FeatureCard.vue'

export default {
  name: 'FeaturesSection',
  components: {
    FeatureCard
  },
  data() {
    return {
      features: [
        {
          icon: 'bi-shield-check',
          title: 'Qualidade Certificada',
          text: 'Todos os nossos equipamentos passam por rigorosos testes de qualidade e possuem certificação ANVISA.'
        },
        {
          icon: 'bi-gear',
          title: 'Tecnologia Avançada',
          text: 'Utilizamos as mais recentes inovações em radiologia digital para garantir precisão nos diagnósticos.'
        },
        {
          icon: 'bi-headset',
          title: 'Suporte Especializado',
          text: 'Nossa equipe de especialistas está disponível 24/7 para auxiliar em qualquer necessidade técnica.'
        }
      ]
    }
  }
}
</script>`