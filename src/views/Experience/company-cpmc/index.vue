<template>
  <RowContent
    align="right"
    label="上海协进教育投资有限公司"
    :label-bold="true"
    :label-width="220"
    :is-wrap="true"
    :is-title="true"
    text="2020年9月——2022年3月"
  />

  <ListWrap title="工作内容与职责：" :list="list" inner titleSize="base" bold />

  <ProMain />
</template>

<script setup lang="ts">
import { ref } from "vue";
import RowContent from "../../../components/RowContent/RowContent.vue";
import ListWrap from "../../../components/ListWrap/ListWrap.vue";
import ProMain from "./ProMain.vue";

const list = ref([
  "负责框架的选型与研发，从零到一构建UCMT学习平台相关系统",
  "根据设计图切图，以页为模块单位完成相关静态页的开发",
  "将页面各子模块组件化，维护容器组件及其展示组件",
  "各子页面进行移动端响应式适配和其他兼容处理",
]);
</script>
