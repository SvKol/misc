<script setup>
const options = ref([
  {id:'OR', number:1, fruit:'Oranges', color:'orange'},
  {id:'BN', number:2, fruit:'Bananas', color:'yellow'},
  {id:'AP', number:3, fruit:'Apples', color:'red'},
])

const selected = ref()
</script>

<template>
  <div class="flex flex-col items-center justify-center w-full h-screen">
    <div class="w-[20rem]">
      <USelectMenu v-model="selected" :options="options" value-attribute="number" option-attribute="fruit" />
    </div>
  </div>
</template>
