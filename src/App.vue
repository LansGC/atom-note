<template lang="pug">
.atom-note.flex.w-full
  Aside
  .main.flex-1
    OperateBar
    router-view
  Welcome
  Update(version="0.1.0-beta")
</template>

<script setup lang="ts">
import Aside from '@/components/aside.vue'
import Welcome from '@/components/welcome.vue'
import Update from '@/components/update.vue'
import OperateBar from '@/components/operate-bar/index.vue'
</script>

<style lang="scss" scoped>
.main {
  background: var(--el-bg-color);
  width: calc(100vw - 56px);
}
</style>