<script setup lang="ts">
import { ref } from 'vue'

const count = ref(0)
</script>

<template>
  <div class="home">
    <van-nav-bar title="首页" />
    <van-cell-group inset style="margin-top: 16px">
      <van-cell title="当前计数" :value="String(count)" />
    </van-cell-group>
    <div class="btn-group">
      <van-button type="primary" @click="count++">点击 +1</van-button>
      <van-button type="default" @click="count = 0">重置</van-button>
    </div>
  </div>
</template>

<style scoped>
.btn-group {
  display: flex;
  justify-content: center;
  gap: 12px;
  margin-top: 24px;
}
</style>
