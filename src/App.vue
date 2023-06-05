<script setup lang="ts">
    type TODO = {
        id: number;
        status: "todo" | "in_progress" | "done";
        title: string;
        description: string;
    };

    const data: TODO[] = [
        {
            id: 1,
            status: "todo",
            title: "TODO 1",
            description: `Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.`,
        },
        {
            id: 2,
            status: "in_progress",
            title: "TODO 2",
            description: `Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.`,
        },
        {
            id: 3,
            status: "done",
            title: "TODO 3",
            description: `Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.`,
        },
    ];
</script>

<template>
    <pre>
        {{ JSON.stringify(data, null, 2) }}
    </pre>
</template>

<style scoped>
</style>
