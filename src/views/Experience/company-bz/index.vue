<template>
  <RowContent
    align="right"
    label="上海宝尊电子商务有限公司"
    :label-bold="true"
    :label-width="220"
    :is-wrap="true"
    :is-title="true"
    text="2022年3月——至今"
  />

  <ListWrap
    title="工作内容与职责："
    :list="list"
    inner
    title-size="base"
    bold
  />

  <ListWrap title="主要成果" :list="fruitList" inner title-size="base" bold />

  <ProUmi />
  <ProNext />
  <ProTeam />
</template>

<script setup lang="ts">
import { ref } from "vue";
import RowContent from "../../../components/RowContent/RowContent.vue";
import ListWrap from "../../../components/ListWrap/ListWrap.vue";
import ProUmi from "./ProUmi.vue";
import ProNext from "./ProNext.vue";
import ProTeam from "./ProTeam.vue";

const list = ref([
  "负责项目前端架构设计，确定技术选型，制定并推进团队的开发规范；",
  "梳理产品需求文档，编写高质量的开发文档，促进团队协作与知识共享；",
  "配合设计团队高效完成前端开发，实现产品功能并满足客户需求；",
  "与后端工程师协作，制定并优化数据接口，确保前后端高效交互；",
  "负责项目需求开发、自测及 Code Review，及时反馈并解决测试阶段的问题。",
]);

const fruitList = ref([
  "基于 Ant Design 封装表单组件 LightForm，有效提升开发效率。该组件借鉴了 form-render 开源项目的理念，但并未完全沿用其实现方式，而是结合 Ant Design 进行二次封装，使其能够通过 JSON 简单配置快速渲染表单页面。",
  "在 LightForm 的基础上，进一步扩展出 ModalForm、LightSearch、LightTable、LightPage 等组件，并在多个项目中成功应用，提升开发的灵活性和复用性。",
  "负责 Weisas 智慧商城项目的促销、营销、分销、消息等核心模块的重构与开发，优化系统功能与性能。",
  "主导 Weisas 智慧商城基础架构的重构，将原有的 dva 状态管理替换为 React Context，优化代码结构，提升可维护性，并增强问题溯源能力。",
  "定期组织 Code Review 和技术分享，促进团队技术沉淀与高效协作。",
]);
</script>

<style scoped></style>
