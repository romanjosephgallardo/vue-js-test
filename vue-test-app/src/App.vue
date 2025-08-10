<script setup>
	import { ref } from "vue";
	let count = ref(0);
</script>

<template>
    <h1> Count: {{  count  }}</h1>
	<button @click="count++"> + </button>
	<button @click="count--"> - </button>
</template>
 
<style></style>