<template>
  <div class="relative bg-gray-50 overflow-hidden">
    <div class="relative pt-6 pb-12 sm:pb-16">
      <div class="max-w-screen-xl mx-auto px-4 sm:px-6">
        <nav
          class="relative flex items-center justify-between sm:h-10 md:justify-between"
        >
          <div class="hidden md:flex md:space-x-10">
            <nuxt-link
              to="/"
              class="font-medium text-primary-500 hover:text-gray-500 transition duration-150 ease-in-out"
              >Home</nuxt-link
            >
            <nuxt-link
              to="/portfolio"
              class="font-medium text-primary-500 hover:text-gray-500 transition duration-150 ease-in-out"
              >Portfolio</nuxt-link
            >
            <nuxt-link
              class="font-medium text-primary-500 hover:text-gray-500 transition duration-150 ease-in-out"
              to="/games"
            >
              Games
            </nuxt-link>
            <nuxt-link
              to="/blog"
              class="font-medium text-primary-500 hover:text-gray-500 transition duration-150 ease-in-out"
              >Blog</nuxt-link
            ><nuxt-link
              class="font-medium text-primary-500 hover:text-gray-500 transition duration-150 ease-in-out"
              to="/contact"
            >
              Contact
            </nuxt-link>
          </div>
          <div>
            <SocialMediaFooter></SocialMediaFooter>
          </div>
        </nav>
      </div>
    </div>
  </div>
</template>

<script>
import SocialMediaFooter from '@/components/SocialMediaFooter'
export default {
  components: { SocialMediaFooter },
}
</script>

<style></style>
