<script setup>
import { ref } from "vue";

const test = ref("test");

setTimeout(() => {
  test.value = "test2";
},2000)

</script>

<template>
  
  <p class="special"
  :key="test"
  >
  {{ test }} 
  </p>
</template>

<style scoped>
.container-1 {
  border: 2px red solid;
}

.container-2 {
  border: 2px skyblue solid;
}

.special {
  font-size: 30px;
  animation: openin 0.5s ease-in-out;
}

@keyframes openin {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}

</style>
