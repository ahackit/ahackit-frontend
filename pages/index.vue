<template>
  <div class="xl:container mx-auto flex">
    <div class="flex items-center justify-center flex-grow space-x-5">
      <div class="flex flex-col space-y-1">
        <p>Hi! My name is</p>
        <p class="text-primary-500 text-4xl align-middle font-bold">
          Austin Hackett
        </p>
        <p class="text-2xl">
          I'm a
          <span class="text-primary-500 font-bold"
            >Fullstack Web Developer</span
          >
        </p>
        <p>
          I'm currently building applications with
          <span class="text-primary-500 font-bold">Javascript</span>
          and
          <span class="text-primary-500 font-bold">Python</span>
        </p>
        <nuxt-link
          to="/portfolio"
          class="bg-green-500 hover:bg-purple-700 text-white py-2 px-4 rounded w-1/3 text-center"
          >See My Work</nuxt-link
        >
      </div>
      <img
        class="object-scale-down h-56 rounded-full"
        src="~/assets/profile.jpg"
        alt="My ugly mug"
      />
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
@apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
</style>
