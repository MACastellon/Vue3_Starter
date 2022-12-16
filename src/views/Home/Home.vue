<script setup lang="ts">
import { useCounterStore } from '@/stores/counter';
const counter = useCounterStore();
</script>

<template>
    <div class="w-100 flex h-screen flex-col items-center justify-center bg-gradient-to-r from-green-500 to-blue-500">
        <div class="mb-4 text-center text-white">
            <h1 class="w-100 mb-3 text-5xl font-bold">Vue3 + Typescript + Tailwindcss Starter</h1>
            <h2 class="mb-3 text-4xl">Vue router + Pinia included</h2>
            <h3 class="text-3xl">Powered by Vite &#9889;</h3>
        </div>
        <div class="text-center text-white">
            <div class="text-lg">Counter: {{ counter.count }}</div>
            <button class="mt-2 rounded-full bg-green-500 px-3 py-1" @click="counter.increment">Increase</button>
        </div>
    </div>
</template>
