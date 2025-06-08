<script setup lang="ts">
    const mesas: {
        name: string,
        status: number
    }[] = await $fetch("http://localhost:3001/mesas")
</script>

<template>
    <Mesa
        v-for="mesa in mesas"
        :name="mesa.name"
        :status="mesa.status" />
</template>