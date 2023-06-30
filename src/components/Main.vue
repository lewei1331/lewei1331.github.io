<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
<div id="mainapp">
    <h1>{{ msg }}</h1>
</div>
</template>


<style scoped>
.read-the-docs {
  color: #888;
}
</style>
