<template>
  <div class="flex flex-col rounded-lg shadow-lg overflow-hidden">
    <div class="flex-shrink-0">
      <img
        class="h-48 w-full object-cover"
        src="https://images.unsplash.com/photo-1496128858413-b36217c2ce36?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1679&q=80"
        alt
      />
    </div>
    <div class="flex-1 bg-white p-6 flex flex-col justify-between">
      <div class="flex-1">
        <!-- <p class="text-sm leading-5 font-medium text-indigo-600">
          <a href="#" class="hover:underline">Blog</a>
        </p> -->
        <a href="#" class="block">
          <h3 class="mt-2 text-xl leading-7 font-semibold text-primary-500">
            Boost your conversion rate
          </h3>
          <p class="mt-3 text-base leading-6 text-gray-500">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Architecto
            accusantium praesentium eius, ut atque fuga culpa, similique sequi
            cum eos quis dolorum.
          </p>
        </a>
      </div>
      <h1 class="mt-6 text-primary-500">Technologies</h1>
      <div class="flex items-center">
        <TechIcon tech-title="Django" img-src="djangoicon"></TechIcon>
      </div>
    </div>
  </div>
</template>

<script>
import TechIcon from '@/components/TechIcon'
export default {
  name: 'Card',
  components: [TechIcon],
}
</script>

<style></style>
