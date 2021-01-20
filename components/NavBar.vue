<template>
  <div class="relative bg-gray-50">
    <div class="relative pt-6 pb-12 sm:pb-16">
      <div class="max-w-screen-xl mx-auto md:px-4">
        <nav
          class="relative flex items-center justify-between sm:h-10 md:justify-between"
        >
          <button
            class="md:hidden inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-white hover:bg-gray-700 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-white"
            aria-expanded="false"
            @click="openMobileMenu"
          >
            <span class="sr-only">Open main menu</span>
            <!-- Icon when menu is closed. -->
            <!--
            Heroicon name: menu

            Menu open: "hidden", Menu closed: "block"
          -->
            <svg
              v-if="!mobileMenuOpen"
              class="block h-6 w-6"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
              aria-hidden="true"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M4 6h16M4 12h16M4 18h16"
              />
            </svg>
            <!-- Icon when menu is open. -->
            <!--
            Heroicon name: x

            Menu open: "block", Menu closed: "hidden"
          -->
            <svg
              v-else
              class="block h-6 w-6"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
              aria-hidden="true"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M6 18L18 6M6 6l12 12"
              />
            </svg>
          </button>
          <div class="hidden md:flex relative justify-between w-screen">
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
              <!-- <nuxt-link
              to="/blog"
              class="font-medium text-primary-500 hover:text-gray-500 transition duration-150 ease-in-out"
              >Blog</nuxt-link
            > -->
              <nuxt-link
                class="font-medium text-primary-500 hover:text-gray-500 transition duration-150 ease-in-out"
                to="/contact"
              >
                Contact
              </nuxt-link>
            </div>
            <div class="hidden md:block">
              <SocialMediaFooter></SocialMediaFooter>
            </div>
          </div>
        </nav>
        <div
          v-if="mobileMenuOpen"
          class="md:hidden absolute flex-col w-screen h-screen bg-gray-800"
        >
          <nuxt-link
            to="/"
            class="block mb-2 font-medium text-center text-primary-500 hover:text-gray-500 transition duration-150 ease-in-out"
            >Home</nuxt-link
          >
          <nuxt-link
            to="/portfolio"
            class="block mb-2 font-medium text-center text-primary-500 hover:text-gray-500 transition duration-150 ease-in-out"
            >Portfolio</nuxt-link
          >
          <!-- <nuxt-link
              to="/blog"
              class="font-medium text-primary-500 hover:text-gray-500 transition duration-150 ease-in-out"
              >Blog</nuxt-link
            > -->
          <nuxt-link
            class="block mb-2 font-medium text-center text-primary-500 hover:text-gray-500 transition duration-150 ease-in-out"
            to="/contact"
          >
            Contact
          </nuxt-link>
          <div class="flex justify-center">
            <SocialMediaFooter class="self-center"></SocialMediaFooter>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import SocialMediaFooter from '@/components/SocialMediaFooter'
export default {
  components: { SocialMediaFooter },
  data() {
    return {
      mobileMenuOpen: false,
    }
  },
  methods: {
    openMobileMenu() {
      this.mobileMenuOpen = !this.mobileMenuOpen
    },
  },
}
</script>

<style></style>
