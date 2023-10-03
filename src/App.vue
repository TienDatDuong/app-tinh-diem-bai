<script setup lang="ts">
import AppTinhTien from "./components/AppTinhTien.vue";
import HeaderApp from "./views/header-app/index.vue";
</script>

<template>
  <div class="h-100% w-100%">
    <app-tinh-tien>
      <template #header>
        <header-app class="h-50px" />
        <n-divider />
      </template>
    </app-tinh-tien>
  </div>
</template>

<style scoped>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
</style>
