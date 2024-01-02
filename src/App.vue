<script setup>
// //导入函数
// import { reactive } from 'vue';

// //执行函数 传入对象类型参数 变量接受
// const state = reactive({
//   count:0
// })
// const setCount = ()=>{
//   state.count++
// }
//导入函数
import { ref } from 'vue'
//执行函数 传入参数【简单类型 对象类型】 变量接受
const count = ref({
  count:0
})
const setCount = ()=>{
  //修改数据需要加.value
  count.value++
}
</script>

<template>
  <div>
    <!-- <button @click="setCount">{{ state.count }}</button> -->
    <button @click="setCount">{{ count.value }}</button>
  </div>
</template>