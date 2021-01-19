<template>
  <div class="xl:container mx-auto flex-column justify-around text-center">
    <h1 class="text-2xl mb-4 font-bold">Currently adding projects</h1>
    <p>
      Below you will find a few of the projects that I've worked on or built.
    </p>
    <nuxt-link class="text-primary-500" to="contact"
      >Interested in hearing about customer projects?</nuxt-link
    >
    <div class="flex flex-col space-y-4">
      <Card
        :image="'vue_deckgl'"
        :title="'Vue_DeckGL'"
        link="https://github.com/loftylabs/vue_deckgl"
      >
        <p class="font-bold text-gray-700">
          An open-source project maintained by the team at Lofty that builds Vue
          bindings on top of Uber's DeckGL library
        </p>
      </Card>
    </div>
  </div>
</template>

<script>
// import Card from '@/components/Card'
export default {
  // components: { Card },
}
</script>

<style></style>
