<template>
    <p> First Name: {{  props.firstName }}</p>
    <p> Last Name: {{ props.lastName }}</p>
</template>

<script setup>
    const props = defineProps(['firstName', 'lastName'])
</script>

<style lang="scss" scoped>

</style>