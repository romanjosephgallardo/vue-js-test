<template>
    <DynamicPropsComponent 
        :firstName="firstName"
        :lastName="lastName"
    />
</template>

<script setup>
    import { ref } from "vue";
    import DynamicPropsComponent from "./DynamicPropsComponent.vue";
    const firstName = ref('Alex');
    const lastName = ref('Gonzales');
</script>

<style lang="scss" scoped>

</style>