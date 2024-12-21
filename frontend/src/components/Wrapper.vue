<script setup lang="ts">
</script>

<template>
    <div class="wrapper">
        <div class="header">
            <slot name="header"></slot>
        </div>
        <div class="content">
            <slot name="content"></slot>
        </div>
    </div>
</template>

<style scoped>
.wrapper {
    display: flex;
    flex-direction: column;
}

.header {
    padding: 1rem;
    width: 100%;
    border-bottom: 1px solid var(--color-border);
}

.content {
    padding: 1rem;
}
</style>