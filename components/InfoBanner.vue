<template>
    <section class="py-12 bg-gradient-to-b from-orange-600 to-yellow-600">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <div v-for="feature in data" :key="feature.line1">
                    <div class="text-center flex flex-col justify-center items-center">
                        <component v-bind:is="feature.icon" class="h-14 w-14 mb-4"></component>
                        <span class="text-lg font-bold">{{ feature.line1 }}</span>
                        <span class="text-lg font-semibold">{{ feature.line2 }}</span>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup lang="ts">
import { CalendarIcon, MapPinIcon, CreditCardIcon } from '@heroicons/vue/24/solid'

const data = [
    {
        icon: CalendarIcon,
        line1: 'Sábado 11 de Noviembre',
        line2: '9:00 A.M.'
    },
    {
        icon: MapPinIcon,
        line1: 'Iglesia Rompiendo Fronteras',
        line2: 'Tegucigalpa, Honduras'
    },
    {
        icon: CreditCardIcon,
        line1: 'Inscripción',
        line2: 'L 200'
    },
]
</script>