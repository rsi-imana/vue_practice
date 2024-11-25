<script setup lang="ts">
import { ref } from 'vue'
const selectedOption = ref("A");
</script>

<template>
    <h1>If</h1>
    <p>選択：{{ selectedOption }}</p>

    <div>
        <label for=""><input type="radio" name="" id="" v-model="selectedOption" value="A">A</label>
        <label for=""><input type="radio" name="" id="" v-model="selectedOption" value="B">B</label>
        <label for=""><input type="radio" name="" id="" v-model="selectedOption" value="C">C</label>
    </div>
</template>

<style scoped></style>