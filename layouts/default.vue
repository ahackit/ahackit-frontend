<template>
  <div class="flex flex-col min-h-screen bg-gray-800 text-white">
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
