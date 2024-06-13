<script setup lang="ts">
import Card from './Card.vue';
const cards = [
  { url: 'https://i.imgur.com/unmma82.jpeg', title: 'This is short title' },
  { url: 'https://i.imgur.com/2MM9Jqo.png', title: 'This is very long long long long long long long long long long title' }
]
</script>

<template>
  <div class="content-wrapper">
    <h1>Photo Cards:</h1>
    <div class="content-cards">
      <Card v-for="card in 100" :key="card"
        :card="card === 0 || card % 2 === 0 ? cards[1] : cards[0]"></Card>
    </div>

  </div>
</template>

<style lang="scss" scoped>
.content {
  &-wrapper {
    padding: 0 32px;
    margin-top: 1rem;

  }

  &-cards {
    display: flex;
    gap: 1rem;
    flex-wrap: wrap;
  }
}
</style>
