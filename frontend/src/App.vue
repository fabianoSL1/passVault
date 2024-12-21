<script setup lang="ts">
  import Container from "./components/Container.vue"
  import WebSiteList from "./components/WebSiteList.vue"
  import CredentalList from "./components/CredentialList.vue"
</script>

<template>
  <Container>
    <template #left>
      <WebSiteList />
    </template>
    <template #right>
      <CredentalList />
    </template>
  </Container>
</template>

<style scoped>
.flex {
  display: flex;
  flex-direction: column;
}
</style>
