<template>
  <div>
    <NuxtWelcome />
    <div class="ss"
      v-for="item in items"
      :key="item.id"
    >
      {{ item }}
      <div class="bb">
        bb
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">

import { ref } from 'vue'

const items = ref([1,2,3,4])

</script>

<style lang="scss">
.ss {
  font-size: 100px;
}

.bb {
  font-size: 10px;
  color: #fff;
  margin-top: 10px;
  margin-bottom: 10px;
}
</style>
