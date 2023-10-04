<template>
  <div class="h-50px w-full container-color-violet sticky p0 m0">
    <n-grid :cols="5" responsive="screen" class="inline-block">
      <n-grid-item>
        <icon icon="mdi:information-variant" class="ml-2 color-#fff h-50px" />
      </n-grid-item>
      <n-grid-item span="3" class="pt-3 font-italic text-18px text-center">
        <span class="ma">Bảng Phong Thần</span>
      </n-grid-item>
      <n-grid-item class="text-end">
        <icon
          icon="uil:setting"
          class="mr-2 size-24px color-#fff h-50px"
          @click="handleCreate()" />
      </n-grid-item>
    </n-grid>
  </div>
</template>
<script setup lang="ts">
import { Icon } from "@iconify/vue";

defineProps<{
  handleCreate: Function;
}>();
</script>
