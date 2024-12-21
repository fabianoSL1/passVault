<script setup lang="ts">
    interface Props {
        type: string;
        placeholder: string;
    }

    defineProps<Props>()
</script>

<template>
    <input class="base" :type="type" :placeholder="placeholder">
</template>

<style scoped>
.base {
    color: var(--color-text);
    background-color: var(--color-background);
    border: 1px solid var(--color-background);
    width: 100%;
    border-radius: .5rem;
    padding: .75rem;
    transition: outline .3s;
    outline-color: var(--color-text);
}

.base:focus,
.base:focus-visible,
.base:focus-within {
    outline-style: solid;
    outline-offset: 2px;
}



</style>