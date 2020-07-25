<template>
  <div class="xl:container mx-auto">
    <div class="flex items-center flex-col">
      <img
        class="h-56 rounded-full object-center"
        src="~/assets/profile.jpg"
        alt="My ugly mug"
      />
      <h1 class="text-4xl align-middle">Austin Hackett</h1>
      <h2 class="text-2xl">
        A <span>Fullstack Web Developer</span> building applications with
        <span>Javascript</span> and
        <span>Python</span>
      </h2>
      <h2 class="text-2xl">
        My stack is currently using
      </h2>
      <uL>
        <li>Django</li>
        <li>Vue/Nuxt</li>
        <li>Docker/Kubernetes</li>
        <li>AWS</li>
      </uL>
      <p></p>
      <div class="flex">
        <a
          class="bg-purple-500 hover:bg-purple-700 text-white py-2 px-4 rounded"
        >
          See My Work
        </a>
      </div>
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
