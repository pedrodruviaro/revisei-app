<script setup lang="ts">
useHead({
  titleTemplate: (chunk) => {
    return chunk ? `${chunk} - Revisei` : "Revisei"
  },
})
</script>

<template>
  <div>
    <NuxtLayout>
      <NuxtPage />
    </NuxtLayout>
  </div>
</template>
