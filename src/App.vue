<script setup>
  import { ref } from 'vue'
  import sonCom from './son-com.vue';
  const count = ref(100)
  setTimeout(() => {
    count.value++
  }, 3000);
</script>
<template>
  <div>
    <sonCom :count="count" message="hello"/>
  </div>
</template>