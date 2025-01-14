<template>
    <div>
        <p>Counter: {{ count }}</p>
        <button @click="Increment">Increment</button>&nbsp;
        <button @click="Decrement">Decrement</button>
    </div>
</template>

<script setup>
import { ref } from 'vue';

const count=ref(0)

function Increment() {
    count.value++
}

function Decrement(){
    count.value--
}
</script>

<style scoped>
div{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

p{
    text-align: center;
}
</style>