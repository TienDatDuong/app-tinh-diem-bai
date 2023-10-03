<template>
  <div>
    <n-grid :cols="5" responsive="screen" >
      <n-grid-item class="h-50px">
        <icon icon="mdi:information-variant" class="h-50px ml-2 color-#fff" />
      </n-grid-item>
      <n-grid-item span="3" class="h-50px pt-3 font-bold text-18px text-center">
        <span class="ma">Bảng Phong Thần</span>
      </n-grid-item>
      <n-grid-item class="h-50px text-end">
        <icon icon="uil:setting"  class="h-50px mr-2 size-18px color-#fff"/>
      </n-grid-item>
    </n-grid>
    
  </div>
</template>s
<script setup lang="ts">
import { Icon } from "@iconify/vue";
</script>
