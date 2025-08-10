<template>
    <StudentComponent />

</template>

<script setup>
    import { provide } from 'vue'
    import StudentComponent from './StudentComponent.vue';
    
    provide('studentName', 'Alex')
    provide('studentAge', 20)
    provide('studentLocation', ['Earth', 'IDK'])
</script>

<style lang="scss" scoped>

</style>