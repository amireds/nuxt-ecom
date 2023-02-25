<script setup>
definePageMeta({
  layout: "products",
});

// Fetch the products
const {
  data: products,
  error,
  pending,
} = await useFetch("https://fakestoreapi.com/products");

useHead({
  title: "Nuxt Dojo | Merch",
  meta: [{ name: "description", content: "Nuxt Dojo Merch" }],
});
</script>

<template>
  <div>
    <div class="grid grid-cols-4 gap-5">
      <div class="" v-for="p in products" :key="p.id">
        <ProductCard :product="p" />
      </div>
    </div>
  </div>
</template>

<style scoped></style>
