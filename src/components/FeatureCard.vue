`<template>
  <div class="feature-card">
    <div class="feature-icon">
      <i :class="'bi ' + icon"></i>
    </div>
    <h4 class="feature-title">{{ title }}</h4>
    <p class="feature-text">{{ text }}</p>
  </div>
</template>

<script>
export default {
  name: 'FeatureCard',
  props: {
    icon: String,
    title: String,
    text: String
  }
}
</script>`