<script setup>
import TestCom from './test-com.vue'
import { onMounted, ref } from 'vue'
const h1Ref = ref(null)
const TestComRef = ref(null)
onMounted(()=>{
  console.log(h1Ref.value);
  console.log(TestComRef.value);
})
</script>
<template>
  <div>
    <h1 ref="h1Ref">hello</h1>
    <TestCom ref="TestComRef"/>
  </div>
</template>