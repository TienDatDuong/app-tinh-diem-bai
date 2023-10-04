<template>

  <n-drawer v-model:show="showModal" :width="502">
    <n-drawer-content title="Stoner" closable>
      Stoner is a 1965 novel by the American writer John Williams.
    </n-drawer-content>
  </n-drawer>
</template>
<script setup lang="ts">
import { ref } from "vue";

const showModal = ref<boolean>(false);


defineExpose({ showModal });
</script>
