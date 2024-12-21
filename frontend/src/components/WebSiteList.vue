<script setup lang="ts">
import BaseButton from "./BaseButton.vue"
import BaseInput from "./BaseInput.vue";
import Wrapper from "./Wrapper.vue"
    const websites = ["Netflix", "Githux"]
</script>

<template>
    <Wrapper>
        <template #header>
            <div style="display: flex; height: 100%;">
                <div style="align-self: center; width: 100%;">
                    <BaseInput type="text" placeholder="filtro"></BaseInput>
                </div>
            </div>
        </template>
        <template #content>
            <BaseButton v-for="website in websites">{{ website }}</BaseButton>
        </template>
    </Wrapper>
</template>

<style scoped>
</style>