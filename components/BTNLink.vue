<script setup lang="ts">
const { link } = defineProps({
  link: String,
});
</script>

<template>
  <NuxtLink
    :to="link"
    class="px-5 py-2 text-base border-[#9854f1] bg-[#9854f1] text-white rounded-lg border hover:border-purple-400 hover:bg-purple-400 cursor-pointer inline-flex items-center justify-center outline-none relative focus:outline-none button-shadow">
    <span class="flex items-center justify-center">
      <slot></slot>
      <SVGFlecha />
    </span>
  </NuxtLink>
</template>
