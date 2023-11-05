<template>
    <section class="py-12 bg-black">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-3 gap-24">
                <div v-for="feature in data" :key="feature.line1">
                    <div class="text-center text-white flex flex-col justify-center items-center">
                        <component v-bind:is="feature.icon" class="h-14 w-14 mb-8 text-orange-500"></component>
                        <span class="text-lg font-bold">{{ feature.line1 }}</span>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup lang="ts">
import { ArrowRightCircleIcon, FireIcon, UserGroupIcon } from '@heroicons/vue/24/solid'

const data = [
    {
        icon: ArrowRightCircleIcon,
        line1: 'Aprende a alcanzar las nuevas generaciones',
    },
    {
        icon: FireIcon,
        line1: 'Sé impartido en el poder de sanidades y milagros',
    },
    {
        icon: UserGroupIcon,
        line1: 'Aprende cómo discipular multitudes',
    },
]
</script>