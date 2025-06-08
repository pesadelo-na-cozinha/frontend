<script setup lang="ts">
    const props = defineProps<{
        name: string
        status: number
    }>()

    const name = props.name
    const status = props.status
</script>

<template>
    <div>
        <h1>{{ name }}</h1>
        <h5>{{ status }}</h5>
    </div>
</template>

<style scoped>
    div {
        border: 1px solid black;
        display: inline-block;
        margin: 10px;
        padding: 10px;
    }
</style>