<script setup>
import sonCom from './son-com.vue';
const getMessage = (msg) => {
  console.log(msg);
}
</script>
<template>
  <div>
    <sonCom @get-message="getMessage" />
  </div>
</template>