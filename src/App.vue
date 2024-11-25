<script setup lang="ts">
import If from './components/If.vue';
import For from './components/For.vue';
import Comp01 from './components/Comp01.vue';
import Comp02 from './components/Comp02.vue';
import { ref } from 'vue';

const showFlg = ref(false);

const showComponent = () => {
  showFlg.value = !showFlg.value;
}
</script>

<template>
  <Comp01></Comp01>
  <Comp01>
    <p>これが引き継がれる</p>
  </Comp01>

  <Comp02 title="title01" content="content01"></Comp02>

<!-- <button @click="showComponent">Show Component</button>
  <HelloWorld v-if="showFlg"></HelloWorld> -->

  <!-- <If></If>
  <br>
  <For></For> -->
</template>

<style scoped>
</style>