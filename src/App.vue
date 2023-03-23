<script setup lang="ts">
import { ref } from 'vue';
import Counter from './components/Counter.vue'

const count = ref(0)
</script>
<template>
    <div>
        <Counter :count="count" @increment="count++" />
    </div>
</template>