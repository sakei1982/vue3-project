<script setup>
import { ref } from 'vue'
import { computed } from 'vue';
const list = ref([1, 2, 3, 4, 5, 6, 7, 8])
const computedList = computed(() => {
  return list.value.filter(item => item > 2)
})
setTimeout(() => {
  list.value.push(9,10)
}, 3000);
</script>
<template>
  <div>
    {{ list }}
  </div>
  <br>
  <div>
    {{ computedList }}
  </div>
</template>