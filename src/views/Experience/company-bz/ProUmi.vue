<template>
  <ProjectWrap
    class="pl-4"
    title="Weisas 智慧商城"
    description="Weisas 智慧商城是一款用于 C 端用户的智能电商平台，致力于为企业提供全方位的一站式运营解决方案。平台集成了商品配置、页面定制、分销管理、消息中心、促销活动、营销策略及文章管理等多项功能，通过灵活配置与高效管理，助力企业实现精准营销、优化用户体验，并推动业务迅速增长。在该项目中，我担任前端组长，主要负责 Web 前端的开发与维护工作，确保平台在交互体验与性能表现上始终保持领先。"
  >
    <template #lib>
      <Button plain type="info" size="small">React</Button>
      <Button plain type="info" size="small">Ant Design</Button>
      <Button plain type="info" size="small">Umi</Button>
      <Button plain type="info" size="small">React-Dnd</Button>
      <Button plain type="info" size="small">Echarts</Button>
      <Button plain type="info" size="small">Lodash</Button>
    </template>
    <ListWrap title="主要贡献：" :list="edrList" inner bold />

    <ListWrap title="项目难点：" :list="hardList" inner bold />
  </ProjectWrap>
</template>

<script setup lang="ts">
import { ref } from "vue";
import ProjectWrap from "../../../components/ProjectWrap/ProjectWrap.vue";
import ListWrap from "../../../components/ListWrap/ListWrap.vue";
import { Button } from "fri-element-plus";

const edrList = ref([
  "负责该项目前端架构的设计与规划，制定统一的团队代码风格，引导团队遵循最佳实践和标准开发流程，同时承担公共组件开发探讨及业务代码 Code Review 等工作；",
  "负责编写公共组件文档，全面提升了团队开发效率；",
  "实现首页安全概览及可配置化展示，大幅提升了用户体验与客户满意度；",
  "完成消息中心模块的开发，使运营人员能够更高效地管理消息，提升了运营效率，并对已发送订阅消息进行规范化留存和管理；",
  "对订单、促销、营销、分销管理等模块进行重构与维护，显著提高了系统的安全性和灵活性。",
]);

const hardList = ref([
  "针对营销、促销等复杂模块的表单开发，直接使用 antd 的 Form 组件往往会导致单个文件中包含会有数百行，极大增加了后续维护和管理的难度。因此，我们对 antd 表单进行了二次封装（LightForm），使开发人员能够通过少量代码快速生成复杂表单；",
  "原有代码采用 dva 进行状态管理，但在接口修改或错误溯源时，常常难以定位变量的来源。为此，我们在后续开发中将 dva 替换为 React Context 进行状态管理，不仅提高了变量溯源能力，还借助 React Hooks 生命周期进行逻辑处理，从而显著提升了开发效率；",
  "由于该项目为 SaaS 产品，涉及多租户环境，常需定制首页、活动页等需求。为满足 C 端页面的个性化定制，我们采用 form-render 数据模型，通过 JSON 配置生成模块组件，并结合 react-dnd 实现拖拽功能，有效提升了页面装修的灵活性和定制化程度。",
]);
</script>
