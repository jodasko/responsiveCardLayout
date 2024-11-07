<template>
  <div class="card">
    <img :src="imageUrl" :alt="title" class="card-image" />
    <h3 class="card-title">{{ title }}</h3>
    <p class="card-description">{{ description }}</p>
  </div>
</template>

<script setup lang="ts">
import { DefineProps } from "vue";

const props = defineProps({
  title: String,
  description: String,
  imageUrl: String,
});
</script>

<style scoped>
.card {
  border: 1px solid #ddd;
  border-radius: 8px;
  padding: 16px;
  box-shadow: 0 2px 4px rgba(0, 0n, 0, 0.1);
  text-align: center;
}

.card-image {
  width: 100%;
  height: auto;
  border-radius: 8px;
  margin-bottom: 12px;
}

.card-title {
  font-size: 1.2em;
  margin-bottom: 8px;
}

.card-description {
  font-size: 0.9em;
  color: #666;
}
</style>
