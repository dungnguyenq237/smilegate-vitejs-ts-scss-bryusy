<script setup lang="ts"></script>

<template>
  <div class="header-wrapper">
    <div class="header-logo">
      <img src="https://i.imgur.com/sOCVfKv.png" alt="logo" />
      Dung Nguyen
    </div>
    <div class="header-actions">
      <button>Indie Game</button>
      <button>Entry Game</button>
      <button>Community</button>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.header {
  &-wrapper {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #94eaa3;
    height: 64px;
    padding: 0 32px;
    position: sticky;
    top: 0;
    z-index: 1;
  }

  &-logo {
    color: white;
    display: flex;
    align-items: center;
    gap: 0.5rem;

    img {
      max-height: 36px;
    }
  }

  &-actions {
    display: flex;
    align-items: center;
    gap: 0.5rem;

    button {
      color: white;
      border: 1px solid white;
      background-color: transparent;
      border-radius: 4px;
      padding: 0.5rem;
      cursor: pointer;

      &:hover {
        opacity: 0.7;
      }
    }
  }
}
</style>
