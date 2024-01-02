<!-- <script>
  export default{
    setup(){
      console.log('setup',this)
      const message = 'thishello'
      const logMessage = () => {
        console.log(message)
      }
      return{
        message,
        logMessage
      }
    },
  beforeCreate(){
    console.log('beforeCreate')
  }
  }
</script> -->
<script setup>
const message = 'this'
const logMessage = () => {
  console.log(message)
}
</script>
<template>
  <div>
    {{ message }}
    <button @click="logMessage">log</button>
  </div>
</template>