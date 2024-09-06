<script setup lang="ts"></script>

<template>
  <header class="border-b border-cool-200 dark:border-cool-800">
    <UContainer
      class="py-4 flex items-center flex-wrap gap-2.5 justify-between"
    >
      <NuxtLink to="/" class="hover:opacity-80 focus:opacity-80 transition-all">
        <Logo />
      </NuxtLink>

      <UButton
        label="Entrar agora"
        icon="i-heroicons-arrow-right-start-on-rectangle-solid"
        size="md"
        trailing
        to="/auth/login"
      />
    </UContainer>
  </header>
</template>
