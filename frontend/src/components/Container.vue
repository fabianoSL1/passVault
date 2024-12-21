<template>
    <div class="container border">
        <div class="divider">
            <div class="left">
                <slot name="left"></slot>
            </div>
            <div class="right">
                <slot name="right"></slot>
            </div>
        </div>
    </div>
</template>

<style scoped>
.container {
    overflow: hidden;
    background-color: var(--color-background-soft);
    width: 100%;
    max-width: 1024px;
    height: 90vh;
}

.border {
    border-radius: 1.5rem;
    transition: border-color .3s;
    border: 1px solid var(--color-border);
}

.divider {
    display: flex;
    height: 100%;
}

.left {
    
    flex-grow: 1;
    border-right: 1px solid var(--color-border);
}

.right {
    flex-grow: 2;
}
</style>
