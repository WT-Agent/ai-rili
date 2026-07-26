<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 138****5500 查询了新科技公司开业剪彩黄金吉时"
  },
  {
    "text": "用户 189****2211 生成了乔迁新居入宅仪式与方位吉时指南"
  },
  {
    "text": "用户 131****8899 完成了霜降节气养生茶饮与心境调适建议"
  },
  {
    "text": "用户 156****3310 生成了重要商业合同签署日冲煞化解"
  },
  {
    "text": "用户 177****4422 取得了每日出行财神方位与注意事项"
  }
]);
</script>
