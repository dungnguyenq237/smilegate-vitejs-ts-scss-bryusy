<script setup lang="ts">
defineProps({
  key: Number,
});
</script>

<template>
  <div class="card-wrapper">
    <img
      :src="
        key % 2 === 0
          ? 'https://imgur.com/2MM9Jqo'
          : 'https://imgur.com/unmma82'
      "
      alt="card-img"
      loading="lazy"
    />
    <div>This is very long card title</div>
  </div>
</template>

<style lang="scss" scoped></style>
