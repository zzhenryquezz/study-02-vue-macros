<script setup lang="ts">

const count = defineProp<number>('count', {
    type: Number,
    default: 0,
})

const increment = defineEmit('increment')

</script>

<template>
    <div>
        <p>Count: {{ count }}</p>
        <button @click="increment">Increment</button>
    </div>
</template>