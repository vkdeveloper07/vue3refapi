<script setup>
import { ref } from 'vue';
const count = ref(0);

function increaseCount(){
  count.value++;
}

function decreaseCount(){
  count.value--;
}
</script>

<template>
  <div class="container">
    <h1>Using ref Api</h1>
    <br>
    <hr>
    <button class="clickbtn" @click="increaseCount">Increase Count</button>
    <button class="clickbtn" @click="decreaseCount">Decrease Count</button>
    <p>The count is {{ count }}</p>
  </div>
</template>

<style scoped>

.container{
  width: 100%;
  border: 2px solid white;
}
.clickbtn{
  display: inline-block;
  height: 40px;
  border-radius: 10px;
  width: 150px;
  margin: 10px;
}
</style>
