<template>
  <div class="home">
    <img alt="Vue logo" src="@/assets/logo.png" />
    <div class="home">{{num}}</div>
    <div>d1222223</div>
    <HelloWorld msg="Hello Vue 3 + Vite" />
    <div class="change" @click="changeNum(100)">
      改变num的值
    </div>
  </div>
</template>

<script setup>
import HelloWorld from '@/components/HelloWorld.vue'
import { ref } from '@vue/reactivity'
let num = ref(122111211)
function changeNum(id){
  console.log(id);
  num.value+=id
}
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
