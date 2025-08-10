<script setup>
	import { computed, ref } from "vue";
	const firstName = ref("Roman");
	const lastName = ref("Gallardo ");
	const fullName = computed(() => firstName.value + " " + lastName.value);
</script>

<template>
    <h1> Full name: {{  fullName  }}</h1>
</template>
 
<style></style>