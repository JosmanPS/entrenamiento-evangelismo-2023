
import type { TypoSectionTitle } from '#build/components';
<template>
  <section class="bg-black py-24">
    <div class="container mx-auto px-4">
      <div class="flex flex-col lg:flex-row gap-12">
        <div class="flex-1 min-w-[60%]">
          <TypoSectionTitle>
            Entrenamiento en el Evangelismo Práctico y Efectivo
          </TypoSectionTitle>
          <div class="text-neutral-400 text-lg mt-12 font-medium">
            <p class="mb-4">
              En este entrenamiento se presentará la estrategia
              <b class="font-bold text-white">Invasión del amor de Dios</b>.
            </p>
            <p class="mb-4">
              Este es un movimiento de oración por personas, familias, salud y
              economía Además es un movimiento de evangelismo internacional
              donde, no solamente se habla de Dios a las personas, sino que
              también se le demuestra el poder sobrenatural que hay en el nombre
              de Jesús.
            </p>
            <p class="mb-4">
              Iniciamos en el año 2008, en Chaco Argentina, junto al pastor
              Jorge Ledesma, y poco a poco fue expandiéndose a más iglesias en
              diferentes países.
            </p>
            <p class="mb-4">
              Con los años, el movimiento fue creciendo y hoy, ha llegado a más
              de 50.000.000 de personas en todo el mundo a través de más de
              2.000.000 de cristianos orando.
            </p>
            <p class="mb-4">
              El proyecto de realiza hoy en día en 5.000 iglesias de 57 países
              de los 5 continentes. El proyecto ha sido traducido en más de 10
              idiomas.
            </p>
            <p>
              Cada vez son más los cristianos que se unen a este proyecto de
              evangelización mundial, viendo el crecimiento en sus iglesias y
              milagros sobrenaturales.
            </p>
          </div>
        </div>
        <div class="flex-1 pt-24">
          <Stat
            v-for="stat in stats"
            :key="stat.caption"
            :number="stat.number"
            :caption="stat.caption"
            class="mb-12"
          />
        </div>
      </div>
      <div class="text-center mt-20">
        <CTAButton />
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
const stats = [
  {
    number: "+50,000",
    caption: "Miembros activos en la Iglesia Cristiana Internacional",
  },
  {
    number: "+50",
    caption: "Naciones usando esta estrategia",
  },
  {
    number: "+10,000",
    caption: "Adolescentes como miembros activos de la Iglesia",
  },
];
</script>