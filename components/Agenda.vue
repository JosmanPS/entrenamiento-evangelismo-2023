<template>
  <section class="pt-24 pb-24">
    <div class="container mx-auto">
      <div class="text-center mb-12">
        <TypoSectionTitle>Agenda</TypoSectionTitle>
      </div>
      <div class="bg-neutral-800 max-w-2xl mx-auto py-12 px-8 rounded-lg">
        <h3 class="text-white font-semibold font-condensed text-xl mb-6">
          Sábado 11 de Noviembre
        </h3>
        <table class="text-primary w-full text-center rounded-xl">
          <thead>
            <tr
              class="font-bold font-condensed text-neutral-400 text-xl border-b-2 p-2"
            >
              <th>HORARIO</th>
              <th>DESCRIPCIÓN</th>
            </tr>
          </thead>
          <tbody>
            <tr
              v-for="item in items"
              :key="item.time"
              class="text-xl font-medium border-b-2 border-neutral-500 text-neutral-300"
              :class="{ 'bg-neutral-700': item.break }"
            >
              <td class="p-4">{{ item.time }}</td>
              <td class="p-4">{{ item.desc }}</td>
            </tr>
          </tbody>
        </table>
      </div>
      <div class="text-center mt-12">
        <CTAButton />
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
const items = [
  { time: "8:30 - 9:00", desc: "REGISTRO", break: true },
  { time: "9:00 - 9:30", desc: "Alabanza y Adoración", break: false },
  { time: "9:30 - 10:30", desc: "Primera Plenaria", break: false },
  { time: "10:30 - 11:00", desc: "COFFEE BREAK", break: true },
  { time: "11:00 - 12:00", desc: "Segunda Plenaria", break: false },
  { time: "12:00 - 12:30", desc: "Ministración", break: false },
];
</script>