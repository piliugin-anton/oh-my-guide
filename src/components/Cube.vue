<template>
  <div class="cube"></div>
</template>

<script setup>

</script>

<style lang="scss" scoped>
.cube {
  width: 64px;
  height: 64px;
  background-color: orange;
  border-radius: 16px;
  border: 2px solid #888;
  transition: transform 0.333s ease-in-out;

  &:hover {
    transform: scale(0.8, 0.8);
  }
}
</style>
