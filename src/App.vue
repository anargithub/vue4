<template>
    <div class="block">
      <draw-column 
        v-model="numOne" 
        :style="{height:`${numOne}%`}">
      </draw-column>
      <get-number 
        body="Описание 1" 
        v-model="numOne">
      </get-number>
      
    </div>

    <div class="block">
      <draw-column 
        v-model="numTwo" 
        :style="{height:`${numTwo}%`}">
      </draw-column>
      <get-number 
        body="Описание 2" 
        v-model="numTwo">
      </get-number>
    </div>
</template>

<script setup lang="ts">
import {ref} from 'vue';
  import GetNumber from '@/components/GetNumber.vue';
  import DrawColumn from '@/components/DrawColumn.vue';
  
  let numOne = ref(1)
  let numTwo = ref(1)

</script>

<style scoped>
.block{
  height: 300px;
  width: 200px;
  border: 1px solid black;
  margin: 10px;
  display: flex;
  flex-direction: column;
  justify-content: end;
}
</style>
