<template>
  <main>
    <div class="column">
      <div class="row" v-for="i in getRandomInt(100, 150)">
        <Cube v-for="i in getRandomInt(10, 15)" />
      </div>
    </div>
  </main>
</template>

<script setup>
import Cube from './components/Cube.vue'

function getRandomInt(min, max) {
    min = Math.ceil(min)
    max = Math.floor(max)

    return Math.floor(Math.random() * (max - min + 1)) + min
}
</script>

<style lang="scss" scoped>
.column {
  display: flex;
  flex-direction: column;
}

.row {
  display: flex;
  flex-direction: row;

  & > * {
    margin: 4px;
  }
}
</style>
