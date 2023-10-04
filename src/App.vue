<script setup lang="ts">
import { defineAsyncComponent, ref } from "vue";
import AppTinhTien from "./components/AppTinhTien.vue";
import HeaderApp from "./views/header-app/index.vue";

const ModalCreate = defineAsyncComponent(
  () => import("./views/modal-create/index.vue")
);

const refModalCreate = ref();

const handleCreate = () => {
  console.log("vao");
  refModalCreate.value.showModal = true;
};
</script>

<template>
  <div>
    <header-app class="border-l" :handle-create="handleCreate" />
    <n-divider class="inline" />
    <app-tinh-tien>
      <template #body>
        <modal-create ref="refModalCreate"  />
      </template>
    </app-tinh-tien>
  </div>
</template>

<style scoped></style>
