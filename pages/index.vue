<script setup lang="ts">
const router = useRouter()

function handleNavigateToLoginPage() {
  router.push("/auth/login")
}

useSeoMeta({
  title: "Mantenha seu carro em dia, sem complicação.",
  description: "Mantenha seu carro em dia, sem complicação.",
})
</script>

<template>
  <div>
    <LandingPageHero @wants-to-login="handleNavigateToLoginPage" />
    <LandingPageFunctionalities />
    <LandingPageAdvantages @wants-to-login="handleNavigateToLoginPage" />
  </div>
</template>
