<script setup lang="ts">
const currentYear = computed(() => new Date().getFullYear())
</script>

<template>
  <footer class="border-t border-cool-200 dark:border-cool-800 py-10 lg:py-16">
    <UContainer>
      <p class="text-center text-sm">
        &copy; Copyright Revisei - {{ currentYear }}
      </p>
    </UContainer>
  </footer>
</template>
