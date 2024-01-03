<script setup>
   const props = defineProps({
        message:String,
        count:Number
    })
    console.log(props);
    console.log(props.count);
</script>
<template>
    <div>
        {{ message }}---{{ count }}
    </div>
</template>