<template>
    <h1> {{ message }}</h1>
    <input 
        v-model="inputText"
        placeholder="Type something..."
    />
</template>

<script setup>
    import { ref, watch } from "vue";

    const message = ref("Hello, Vue!");
    const inputText = ref(" ");

    watch(inputText, (newValue, oldValue) => { 
        message.value = `You typed: ${newValue}`;
    });
</script>

<style lang="scss" scoped>

</style>