<template>
  <div class="flex flex-col min-h-screen">
    <NavBar></NavBar>
    <Nuxt class="flex-grow" />
    <SocialMediaFooter></SocialMediaFooter>
  </div>
</template>

<script>
import NavBar from '@/components/NavBar'
import SocialMediaFooter from '@/components/SocialMediaFooter'
export default {
  components: { NavBar, SocialMediaFooter },
}
</script>
<style></style>
