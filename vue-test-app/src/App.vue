<script setup>
	import { ref } from "vue";
	let userName = ref("");
</script>

<template>
    <h1> Username: {{  userName  }}</h1>
	<button @click="userName = 'jordan'"> Add User </button>
</template>
 
<style></style>