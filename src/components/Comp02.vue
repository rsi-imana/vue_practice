<script setup lang="ts">
// type Props = {
//     title: string;
//     content: string;
// }
// defineProps<Props>();

defineProps<{
    title: string;
    content: string;
}>();


</script>

<template>
    <p>{{ title }}</p>
    <p>{{ content }}</p>
</template>