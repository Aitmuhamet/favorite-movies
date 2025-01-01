<template>
  <form @submit.prevent="">
    <input
      type="text"
      class="search-input"
      placeholder="Search for a movie..."
      v-model="searchMovie"
    />
    <button type="submit">Search</button>
  </form>
</template>

<script setup>
import { ref } from 'vue';

const searchMovie = ref('');
</script>

<style scoped>
.search-input {
  border: 1px solid #e7e7e7;
  width: 100%;
  height: 40px;
  padding: 0 10px;
  margin-bottom: 20px;
  border-radius: 10px;
}
.search-input:hover {
  outline: 1px solid blue;
}
</style>