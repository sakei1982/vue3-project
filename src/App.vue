<script setup>
  import {ref, watch} from 'vue'
  const count = ref(0)
  const name = ref('cp')
  const changeCount = ()=>{
    count.value++
  }
  const changeName = ()=>{
    name.value='pc'
  }
watch([count,name],([newCount,newName],[oldCount,oldName])=>{
  console.log([newCount,newName],[oldCount,oldName]);
},{immediate:true})
</script>

<template>
  <div>
    <button @click="changeCount">{{ count }}</button>
    <button @click="changeName">{{ name }}</button>
  </div>
</template>
