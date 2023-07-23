<template>
  <div>
      <label for="name">Текст</label>
      <p>{{ props.body }}</p>
      <label for="percent">Значение</label>
      <input type="number" id="percent" 
      :value="props.modelValue"
      @input="$emit('update:modelValue', $event.target?.value)">
  </div>
</template>

<script setup lang="ts">
interface Props{
  body:string;
  modelValue:number;
}
const props = defineProps<Props>()
</script>

<style scoped>

</style>