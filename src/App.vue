<template>
  <div class="card-grid">
    <Card
      v-for="(card, index) in cards"
      :key="index"
      :description="card.description"
      :imageUrl="card.imageUrl"
    />
  </div>
</template>

<script setup lang="ts">
import { ref } from "vue";
import Card from "./components/Card.vue";

const cards = ref([
  {
    title: "Card 1",
    description: "This is the first card.",
    imageUrl: "path/to/image1.jpg",
  },
  {
    title: "Card 2",
    description: "This is the second card.",
    imageUrl: "path/to/image2.jpg",
  },
  {
    title: "Card 2",
    description: "This is the second card.",
    imageUrl: "path/to/image2.jpg",
  },
  {
    title: "Card 2",
    description: "This is the second card.",
    imageUrl: "path/to/image2.jpg",
  },
  {
    title: "Card 2",
    description: "This is the second card.",
    imageUrl: "path/to/image2.jpg",
  },
  {
    title: "Card 2",
    description: "This is the second card.",
    imageUrl: "path/to/image2.jpg",
  },
  {
    title: "Card 2",
    description: "This is the second card.",
    imageUrl: "path/to/image2.jpg",
  },
  {
    title: "Card 2",
    description: "This is the second card.",
    imageUrl: "path/to/image2.jpg",
  },
  {
    title: "Card 2",
    description: "This is the second card.",
    imageUrl: "path/to/image2.jpg",
  },
  {
    title: "Card 2",
    description: "This is the second card.",
    imageUrl: "path/to/image2.jpg",
  },
  {
    title: "Card 2",
    description: "This is the second card.",
    imageUrl: "path/to/image2.jpg",
  },
  {
    title: "Card 2",
    description: "This is the second card.",
    imageUrl: "path/to/image2.jpg",
  },
  {
    title: "Card 2",
    description: "This is the second card.",
    imageUrl: "path/to/image2.jpg",
  },
  {
    title: "Card 2",
    description: "This is the second card.",
    imageUrl: "path/to/image2.jpg",
  },
  {
    title: "Card 2",
    description: "This is the second card.",
    imageUrl: "path/to/image2.jpg",
  },
  {
    title: "Card 2",
    description: "This is the second card.",
    imageUrl: "path/to/image2.jpg",
  },
]);
</script>

<style scoped>
.card-grid {
  display: grid;
  gap: 16px;
  grid-template-columns: 1fr;
}

/* Tablet layout */
@media (min-width: 600px) {
  .card-grid {
    grid-template-columns: 1fr 1fr;
  }
}

/* Desktop layout */
@media (min-width: 1024px) {
  .card-grid {
    grid-template-columns: 1fr 1fr 1fr;
  }
}
</style>
