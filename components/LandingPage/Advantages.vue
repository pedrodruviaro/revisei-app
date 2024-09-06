<script setup lang="ts">
const items = [
  {
    title: "“Desempenho Otimizado",
    content:
      "Carros bem mantidos funcionam de maneira mais eficiente e segura, garantindo uma melhor performance e economia de combustível.",
  },
  {
    title: "Redução de Custos",
    content:
      "Manter um registro detalhado de manutenções ajuda a identificar problemas cedo, evitando reparos maiores e mais caros no futuro.",
  },
  {
    title: "Valor de Revenda",
    content:
      "Veículos com um histórico de manutenção em dia tendem a ter um valor de revenda mais alto e atraem mais compradores.",
  },
  {
    title: "Segurança Aumentada",
    content:
      "Revisões regulares garantem que todos os componentes do veículo estejam funcionando corretamente, reduzindo o risco de falhas e acidentes.",
  },
  {
    title: "Tranquilidade",
    content:
      "Com um registro organizado, você nunca mais esquecerá a última manutenção realizada e poderá planejar futuras revisões com mais facilidade.",
  },
  {
    title: "Imagem/Visual",
    content:
      "Infográfico ou imagens que representem as vantagens de uma manutenção regular, como um carro em boas condições vs. um carro com problemas.",
  },
]

const emits = defineEmits<{
  "wants-to-login": []
}>()
</script>

<template>
  <section class="py-14 lg:py-20">
    <UContainer>
      <h2
        class="text-center mx-auto font-bold text-2xl lg:text-3xl text-balance max-w-[30ch] mb-8"
      >
        Vantagens de Manter um Carro com Manutenção em Dia
      </h2>

      <div
        class="grid md:grid-cols-2 lg:grid-cols-3 gap-6 mx-auto max-w-[70rem]"
      >
        <UCard v-for="item in items" :key="item.title">
          <template #header>
            <h3 class="font-bold text-xl">{{ item.title }}</h3>
          </template>

          <div>
            <p>{{ item.content }}</p>
          </div>
        </UCard>
      </div>

      <div class="mt-10 flex justify-center">
        <UButton
          label="Comece agora"
          size="xl"
          @click="emits('wants-to-login')"
        />
      </div>
    </UContainer>
  </section>
</template>
