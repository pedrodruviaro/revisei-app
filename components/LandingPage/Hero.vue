<script setup lang="ts">
const emits = defineEmits<{
  "wants-to-login": []
}>()
</script>

<template>
  <section class="py-20 lg:py-40 relative grid overflow-hidden">
    <UContainer class="z-[2]">
      <h1
        class="font-bold text-2xl lg:text-3xl xl:text-4xl text-balance md:max-w-[60%] mb-3"
      >
        Controle Total do Histórico de Manutenção do Seu Carro
      </h1>
      <p class="text-lg mb-14 max-w-[47ch] text-balance">
        Nunca mais se esqueça de quando foi a última manutenção. Com o
        <strong>Revisei</strong>, você mantém seu veículo sempre pronto para
        rodar.
      </p>
      <UButton
        label="Cadastre-se Agora"
        size="xl"
        @click="emits('wants-to-login')"
      />
    </UContainer>

    <div
      class="absolute w-full h-full z-[1] max-w-[100%] lg:max-w-[30%] xl:max-w-[40%] right-0 opacity-30 lg:opacity-100"
    >
      <img
        src="/images/hero-img.jpg"
        class="w-full h-full object-cover object-center"
        aria-hidden="true"
        alt=""
      />
    </div>
  </section>
</template>
