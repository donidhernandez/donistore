<script setup>
import products from '../data/products.json'
import ProductCard from './components/ProductCard.vue'
</script>

<template>
  <h1 class="text-3xl font-bold underline">Doni Store</h1>
  <section class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 w-full gap-y-5 p-20">
    <ProductCard :product="product" v-for="product in products" :key="product.id" />
  </section>
</template>
