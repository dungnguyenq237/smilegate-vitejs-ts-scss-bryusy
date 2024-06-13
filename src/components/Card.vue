<script setup lang="ts">
type Card = {
  url: string
  title: string
}

type Props = {
  card: Card
}

const props = defineProps<Props>()
</script>

<template>
  <div class="card-wrapper">
    <div class="card-image">
      <img :src="card.url" alt="Image 1" loading="lazy">
    </div>
    <div class="card-content">
      <p :title="card.title">{{ card.title }}</p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.card {
  &-wrapper {
    background-color: white;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    overflow: hidden;
    width: 300px;
  }

  &-image {
    position: relative;
    width: 100%;
    padding-top: 66.66%;
    overflow: hidden;

    img {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
  }

  &-content {
    padding: 0.5rem;
    font-weight: bold;
    font-size: 1rem;

    p {
      white-space: nowrap;
      overflow: hidden;
      text-overflow: ellipsis;
    }
  }
}
</style>
