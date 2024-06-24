<script setup>
import { ref, computed } from 'vue'
import store from './../store';

defineProps({
  msg: String,
})

const test = computed(() => store.state.test)

const count = ref(0)
</script>

<template>
  <h1 class="text-3xl font-bold underline bg-purple-500">
    Hello world! {{ test }}
  </h1>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
