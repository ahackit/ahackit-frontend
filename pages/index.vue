<template>
  <div class="xl:container mx-auto flex-column justify-between">
    <div>
      <p class="text-center">
        Hi! My name is
        <span class="text-primary-500 font-bold">Austin Hackett </span> or
        <span class="text-primary-500 font-bold">@ahackit </span>
      </p>
    </div>
    <div class="flex items-center justify-center flex-grow space-x-5 mt-8">
      <div class="text-center md:flex md:flex-col md:space-y-1">
        <p class="text-2xl">
          I'm a
          <span class="text-primary-500 font-bold"
            >Full Stack Software Engineer</span
          >
        </p>
        <p>
          I'm currently building applications with
          <span class="text-primary-500 font-bold">Javascript</span>,
          <span class="text-primary-500 font-bold">Python</span>
          <br />
          and a whole lot of other things at
          <a
            class="text-primary-500 hover:text-gray-500 font-bold"
            href="https://www.hirelofty.com"
            >Lofty</a
          >!
        </p>
      </div>
      <img
        class="object-scale-down h-56 rounded-full"
        src="~/assets/profile.jpg"
        alt="My ugly mug"
      />
    </div>
    <div class="flex justify-center mt-8">
      <nuxt-link
        to="/portfolio"
        class="bg-green-500 hover:bg-purple-700 text-gray-800 hover:text-white py-2 px-4 rounded w-1/3 text-center font-bold"
        >See My Work</nuxt-link
      >
    </div>
  </div>
</template>

<script>
export default {
  head: {
    title: 'Home Page',
    meta: [
      {
        hid: 'description',
        name: 'description',
        content: 'Austin Hackett lives here',
      },
      {
        hid: 'og:url',
        name: 'og:url',
        content: 'https://www.ahackit.com',
      },
      {
        hid: 'og:type',
        name: 'og:type',
        content: 'article',
      },
      {
        hid: 'og:description',
        name: 'og:description',
        content: 'Austin Hackett lives here',
      },
      {
        hid: 'og:image',
        name: 'og:image',
        content: 'https://www.ahackit.com/_nuxt/assets/profile.jpg',
      },
      {
        hid: 'twitter:card',
        name: 'twitter:card',
        content: 'summary',
      },
      {
        hid: 'twitter:creator',
        name: 'twitter:creator',
        content: 'https://twitter.com/ahackit',
      },
      {
        hid: 'twitter:title',
        name: 'twitter:title',
        content: 'ahackit.com home',
      },
      {
        hid: 'twitter:description',
        name: 'twitter:description',
        content: 'Austin Hackett lives here',
      },
      {
        hid: 'twitter:image',
        name: 'twitter:image',
        content: 'https://www.ahackit.com/_nuxt/assets/profile.jpg',
      },
    ],
  },
}
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
@apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
</style>
