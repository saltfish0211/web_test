<script setup>
import { ref } from "vue";

// const data = "SF test2";
// const text = ref("defult");

// const view = ref(1);
// const changeview = (index) => {
//   view.value = index;
// };
const fordata = [
  1,
  2,
  3,
  4,
  "sad",
  "sdagf",
  "??"
]

</script>

<template>
  <!-- <button v-on:click="changeview(1)">顯示單向綁定</button>
  <button @click="changeview(2)">顯示雙向綁定</button>
  <button @click="changeview(3)">沒有畫面</button>

  <div class="container-1" v-if="view === 1">
    <p>下面是單向綁定</p>
    {{ data }}
  </div>

  <div class="container-2" v-if="view === 2">
    <p>下面是雙向綁定</p>
    <input type="text" v-model="text" />
    <p>{{ text }}</p>
  </div> -->

  <!-- 這邊要注意if else的判斷大多是1對1，要不然就是你的else條件要寫完善一點 -->
  <!-- <div v-if="view !== 1 && view !== 2">沒有畫面</div> -->
  <p v-for="forlist in fordata">
  {{ forlist }}
  </p>
</template>

<style scoped>
.container-1 {
  border: 2px red solid;
}

.container-2 {
  border: 2px skyblue solid;
}
</style>
