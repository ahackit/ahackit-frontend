<template>
  <div class="xl:container mx-auto">
    <div class="flex items-center flex-col space-y-1">
      <img
        class="h-56 rounded-full object-center"
        src="~/assets/profile.jpg"
        alt="My ugly mug"
      />
      <p>Hi! My name is</p>
      <p class="text-4xl align-middle">Austin Hackett</p>
      <p class="text-2xl">
        A
        <span class="font-bold">Fullstack Web Developer</span> building
        applications with <span class="font-bold">Javascript</span> and
        <span class="font-bold">Python</span>
      </p>
      <a class="bg-purple-500 hover:bg-purple-700 text-white py-2 px-4 rounded"
        >See My Work</a
      >
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
