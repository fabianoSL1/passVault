<script setup lang="ts">
    interface ButtonProps {
        label?: String;
    }

    defineProps<ButtonProps>();

</script>

<template>
    <button class="base" >
        <slot> {{ label }}</slot>
    </button>
</template>

<style scoped>
.base {
    color: var(--color-text);
    outline-color: var(--color-text);   
    background-color: var(--color-background);
    border: 1px solid var(--color-background);
    text-decoration: none;
    cursor: pointer;
    transition: border .3s;
    padding: .75rem 1rem;
    border-radius: .5rem;
    font-weight: 700;
    
}

.base:hover {
    border-color: var(--color-border);
}


.base:focus,
.base:focus-visible,
.base:focus-within {
    outline-style: solid;
    outline-offset: 2px;
}
</style>