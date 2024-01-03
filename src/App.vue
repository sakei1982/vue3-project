<!-- <script setup>
import { ref, watch } from 'vue'
const state = ref({ count: 0 })
const changeStateByCount = () => {
  state.value.count++
}
watch(state, () => {
  console.log('发生变化');
},{deep:true})
</script>
<template>
  <div>
    {{ state.count }}
    <button @click="changeStateByCount">count</button>
  </div>
</template> -->
<script setup>
import { ref, watch } from 'vue'
const info = ref({ name: 'cp', age: 18 })
const changeAge = () => {
  info.value.age++
}
watch(
  () => info.value.age,
  () => console.log('发生变化')
)
</script>
<template>
  <div>
    {{ info.age }}
    <button @click="changeAge">bun</button>
  </div>
</template>