<template>
  <div class="xl:container mx-auto flex-column justify-around">
    <div class="flex justify-between space-x-4">
      <div class="w-1/3">
        <h1 class="text-2xl text-center mb-4">Web Applications</h1>
        <div class="flex flex-col space-y-4">
          <Card></Card>
          <Card></Card>
          <Card></Card>
        </div>
      </div>
      <div class="w-1/3">
        <h1 class="text-2xl text-center mb-4">Open Source Projects</h1>
        <div class="flex flex-col space-y-4">
          <Card></Card>
        </div>
      </div>
      <div class="w-1/3">
        <h1 class="text-2xl text-center mb-4">Games</h1>
        <div class="flex flex-col space-y-4">
          <Card></Card>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Card from '@/components/Card'
export default {
  components: { Card },
}
</script>

<style></style>
