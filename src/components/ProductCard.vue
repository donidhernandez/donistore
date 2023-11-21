<script setup>
const { product } = defineProps(['product'])
</script>

<template>
  <div class="max-w-sm w-[350px] p-8 flex flex-col gap-2 shadow-lg rounden-md justify-around">
    <div class="flex justify-center">
      <img class="w-full h-full object-cover" :src="product.image" :alt="product.title" />
    </div>

    <h2 class="text-xl font-semibold">{{ product.title }}</h2>
    <p class="font-light line-clamp-4">{{ product.description }}</p>
    <div class="mt-2">
      <span class="capitalize bg-slate-900 text-white px-5 py-2">{{ product.category }}</span>
    </div>
    <button
      class="bg-indigo-600 text-white py-3 hover:bg-indigo-800 transition-colors duration-300 ease-in cursor-pointer mt-12"
    >
      Ver Producto
    </button>
  </div>
</template>
