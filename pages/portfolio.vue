<template>
  <div class="container mx-auto">
    <h1 class="text-center">Technologies I'm currently using</h1>
    <div class="flex space-x-8 justify-center">
      <TechIcon tech-title="Django" img-src="djangoicon"> </TechIcon>
      <TechIcon tech-title="Vue" img-src="vueicon"> </TechIcon>
      <TechIcon tech-title="Nuxt" img-src="nuxticon"> </TechIcon>
      <TechIcon tech-title="Tailwind" img-src="tailwindicon"> </TechIcon>
      <TechIcon tech-title="Postgres" img-src="postgresicon"> </TechIcon>
      <TechIcon tech-title="Docker" img-src="dockericon"> </TechIcon>
      <TechIcon tech-title="Kubernetes" img-src="k8icon"> </TechIcon>
      <TechIcon tech-title="AWS" img-src="awsicon"> </TechIcon>
    </div></div
></template>

<script>
import TechIcon from '@/components/TechIcon'
export default {
  components: { TechIcon },
}
</script>

<style></style>
