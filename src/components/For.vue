<script setup lang="ts">
import { ref } from "vue";

const sampleArrayInit: string[] = ["item01", "item02", "item03"];
const sampleArray = ref(sampleArrayInit);

type ObjType = {
    [key: string]: string;
}

const sampleObjectInit: ObjType = {
    key1: "value01",
    key2: "value02",
    key3: "value03"
}

const sampleObj = ref(sampleObjectInit);
</script>

<template>
    <h2>Array</h2>
    <ul>
        <li v-for="item in sampleArray" v-bind:key="item">
            {{ item }}
        </li>
    </ul>

    <ul>
        <li v-for="(item, index) in sampleArray" v-bind:key="item">{{ index }}:{{ item }}</li>
    </ul>

    <h2>Obj</h2>
    <ul>
        <li v-for="(value, key) in sampleObj" v-bind:key="value">
            {{ key }}:{{ value }}
        </li>
    </ul>
</template>

<style></style>