<template>
  <div>
    <NavBar></NavBar>
    <Nuxt />
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
