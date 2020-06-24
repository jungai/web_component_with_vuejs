<template>
  <div class="max-w-sm rounded overflow-hidden shadow-lg">
  <img class="w-full" src="https://tailwindcss.com/img/card-top.jpg" alt="Sunset in the mountains">
  <div class="px-6 py-4">
    <div class="font-bold text-xl mb-2">{{ title }}</div>
    <p class="text-gray-700 text-base">
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus quia, nulla! Maiores et perferendis eaque, exercitationem praesentium nihil.
    </p>
  </div>
  <div class="px-6 py-4">
    <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2">#{{ chip1 }}</span>
    <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2">#{{ chip2 }}</span>
    <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700">#{{ chip3 }}</span>
  </div>
</div>
</template>

<script>
export default {
  name: 'JuCard',
  props: {
    title: {
      type: String,
      default: 'Title',
    },
    chip1: {
      type: String,
      default: 'chip1',
    },
    chip2: {
      type: String,
      default: 'chip2',
    },
    chip3: {
      type: String,
      default: 'chip3',
    },
  },
};
</script>

<style lang="scss">
@import "../assets/css/output";
</style>
