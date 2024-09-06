<script setup lang="ts">
const items = [
  {
    label: "Cadastro e Gerenciamento de Carros",
    icon: "i-heroicons-information-circle",
    defaultOpen: true,
    content: "Adicione e edite informações dos seus veículos.",
  },
  {
    label: "Histórico de Manutenção",
    icon: "i-heroicons-circle-stack",
    content:
      "Registre e visualize todas as manutenções realizadas, incluindo quilometragem, data, oficina e detalhes do serviço.",
  },
  {
    label: "Alertas e Notificações",
    icon: "i-heroicons-information-circle",
    content:
      "Receba lembretes sobre manutenções futuras baseados na quilometragem ou tempo.",
  },
  {
    label: "Notas Personalizadas",
    icon: "i-heroicons-pencil-square-solid",
    content: "Adicione observações detalhadas sobre cada serviço realizado.",
  },
]
</script>

<template>
  <section
    class="border-t border-b border-cool-200 dark:border-cool-800 py-14 lg:py-20"
  >
    <UContainer>
      <h2 class="text-center mx-auto font-bold text-2xl lg:text-3xl mb-8">
        O Que Você Pode Fazer com AutoHistória
      </h2>
      <div class="mx-auto w-full max-w-[50rem]">
        <UAccordion :items="items" size="lg" />
      </div>
    </UContainer>
  </section>
</template>
