<template>
  <div class="mt-7 max-w-sm mx-auto text-center card py-20 space-y-7">
    <p class="text-7xl font-bold">{{ error.statusCode }}</p>
    <p class="text-6xl">Ooops.</p>
    <p class="">{{ error.message }}</p>
    <button class="btn" @click="handleClearError">Go Home...</button>
  </div>
</template>

<script setup>
defineProps(["error"]);
const handleClearError = () => clearError({ redirect: "/" });
</script>

<style scoped></style>
