<template>
  <n-modal v-model:show="showModal">
    <n-card
      :style="styleModal"
      :bordered="false"
      size="huge"
      role="dialog"
      aria-modal="true">
      <template #header-extra> Oops! </template>
      Content
      <template #footer> Footer </template>
    </n-card>
  </n-modal>
</template>
<script setup lang="ts">
import { ref } from "vue";

const showModal = ref<boolean>(false);

const styleModal = {
  width: "300px",
  maxHeight: "300px",
  display: "inline-block",
};

defineExpose({ showModal });
</script>
