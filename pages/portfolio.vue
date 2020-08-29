<template>
  <div class="container mx-auto">
    <!-- <div class="flex space-x-8 justify-center">
      <TechIcon tech-title="Django" img-src="djangoicon"></TechIcon>
      <TechIcon tech-title="Vue" img-src="vueicon"></TechIcon>
      <TechIcon tech-title="Nuxt" img-src="nuxticon"></TechIcon>
      <TechIcon tech-title="Tailwind" img-src="tailwindicon"></TechIcon>
      <TechIcon tech-title="Postgres" img-src="postgresicon"></TechIcon>
      <TechIcon tech-title="Docker" img-src="dockericon"></TechIcon>
      <TechIcon tech-title="Kubernetes" img-src="k8icon"></TechIcon>
      <TechIcon tech-title="AWS" img-src="awsicon"></TechIcon>
    </div> -->
    <h1 class="text-2xl text-center">Web Applications</h1>
    <div class="mt-12 grid gap-5 max-w-lg mx-auto lg:grid-cols-3 lg:max-w-none">
      <Card></Card>
      <Card></Card>
      <Card></Card>
    </div>
    <h1 class="mt-12 text-2xl text-center">Tools</h1>
    <div class="mt-12 grid gap-5 max-w-lg mx-auto lg:grid-cols-3 lg:max-w-none">
      <Card></Card>
      <!-- <Card></Card>
      <Card></Card> -->
    </div>
  </div>
</template>

<script>
import Card from '@/components/Card'
export default {
  components: { Card },
}
</script>

<style></style>
