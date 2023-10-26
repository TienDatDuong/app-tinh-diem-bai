<template>
  <n-drawer v-model:show="showModal" :default-width="600">
    <n-drawer-content title="Nhập tên mới quẩy được nha các bạn" closable>
      <span class="hello">
        Stoner is a 1965 novel by the American writer John Williams.
      </span>
    </n-drawer-content>
  </n-drawer>
</template>
<script setup lang="ts">
import { ref } from "vue";

const showModal = ref<boolean>(false);


defineExpose({ showModal });
</script>
<!-- <style lang="scss">
$bgColor: red;

.hello{
  background-color: $bgColor;
}

</style> -->
