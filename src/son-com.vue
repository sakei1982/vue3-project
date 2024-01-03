<script setup>
const emit = defineEmits(['get-message'])
const sendMsg = () => {
    emit('get-message', 'hello')
}
</script>
<template>
    <div>
        <button @click="sendMsg">触发事件</button>
    </div>
</template>