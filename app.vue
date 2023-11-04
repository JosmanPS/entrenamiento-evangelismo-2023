<template>
  <main class="bg-black">
    <Hero />
    <InfoBanner />
    <About />
    <BenefitsBanner />
    <Speaker />
    <Quote />
    <Agenda />
    <Footer />
  </main>
</template>

<script setup lang="ts">
const title = 'Entrenamiento de Evangelismo Sobrenatural'
const description =
  'Capacitación de Evangelismo práctico y efectivo con Cristian Ledesma. 11 de Nov. Tegucigalpa.'
const seoImageUrl =
  'https://evangelismo.escueladeavivamiento.com/img/seo-img.jpg'

useSeoMeta({
  title,
  ogTitle: title,
  description,
  ogDescription: description,
  ogImage: seoImageUrl,
  twitterCard: 'summary_large_image',
})
</script>