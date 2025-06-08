<script setup lang="ts">
    const mesas = [
        {
            name: "Mesa 1", status: 3
        },
        {
            name: "Mesa 2", status: 2
        },
        {
            name: "Mesa 3", status: 1
        },
        {
            name: "Mesa 4", status: 0
        }
    ]
</script>

<template>
    <Mesa
        v-for="mesa in mesas"
        :name="mesa.name"
        :status="mesa.status" />
</template>