<script setup lang="ts">
const router = useRouter()

function handleNavigateToLoginPage() {
  router.push("/auth/login")
}
</script>

<template>
  <div>
    <LandingPageHeader @wants-to-login="handleNavigateToLoginPage" />
    <main>
      <slot />
    </main>
    <LandingPageFooter />
  </div>
</template>
