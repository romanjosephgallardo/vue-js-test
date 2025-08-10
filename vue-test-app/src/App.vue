<script setup>
	import { ref } from "vue";
	let isVisible = ref(true);
</script>

<template>
    <p v-show="isVisible">
		This is a sentence.
	</p>
	<button @click="isVisible != isVisible"> Toggle Visibility </button>
</template>
 
<style></style>