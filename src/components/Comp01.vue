<script setup lang="ts">
import { ref } from 'vue';


const n = ref(0);
const plusOne = () => {
    n.value++;
}
</script>

<template>
    <button @click="plusOne">click!!</button>
    <p>{{ n }}</p>
    <slot>
        <p>デフォルト</p>
    </slot>
</template>