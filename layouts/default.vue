<template>
  <div class="flex flex-col min-h-screen">
    <NavBar></NavBar>
    <Nuxt class="flex-grow" />
  </div>
</template>

<script>
import NavBar from '@/components/NavBar'

export default {
  components: { NavBar },
}
</script>
<style></style>
