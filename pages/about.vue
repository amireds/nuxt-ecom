<script setup>
const { data } = await useFetch("/api/currency/GBP");
</script>

<template>
  <div>
    <h2>About</h2>
    <p>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequuntur
      dolor eligendi, error et fugit hic inventore ipsum rem voluptate
      voluptatibus!
    </p>
    <p>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequuntur
      dolor eligendi, error et fugit hic inventore ipsum rem voluptate
      voluptatibus!
    </p>

    <div class="">{{ data }}</div>
  </div>
</template>

<style scoped>
h2 {
  margin-bottom: 20px;
  font-size: 36px;
}

p {
  margin: 20px 0;
}
</style>
