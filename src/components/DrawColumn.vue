<template>
  <div class="column">
  </div>
</template>

<script setup lang="ts">
import {ref, computed} from 'vue';
interface Draws{
  percent: number;
}
const draws = defineProps<Draws>()

</script>

<style scoped>
  .column{
      height: 30px;
      width: 30px;
      background-color: teal;
      display: flex;
      flex-direction: column;
      justify-content: end;
  }

</style>