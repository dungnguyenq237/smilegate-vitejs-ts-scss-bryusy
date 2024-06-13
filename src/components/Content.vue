<script setup lang="ts">
import Card from './Card.vue';
</script>

<template>
  <div class="content-wrapper">
    <Card v-for="card in 5" :key="card"></Card>
  </div>
</template>

<style lang="scss" scoped></style>
