<script setup lang="ts">
useHead({
  titleTemplate: (chunk) => {
    return chunk ? `${chunk} - Revisei` : "Revisei"
  },
})
</script>

<template>
  <div>
    <NuxtLoadingIndicator />

    <NuxtLayout>
      <NuxtPage />
    </NuxtLayout>
    <UNotifications :ui="{ strategy: 'override', position: 'top-0 right-0' }" />
  </div>
</template>
