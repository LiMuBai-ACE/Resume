<template>
  <ProjectWrap
    class="team-build pl-4"
    title="团队建设"
    :show-lib="false"
    icon="shejiao"
  >
    <TitleDesc
      icon="shejiao"
      :show-icon="false"
      title="Confluence"
      description="公司内部文档平台，主要用于记录需求变更，公共组件，开发文档，代码规范，会议记录等。内容"
    />

    <ListWrap
      title="核心内容："
      :list="teamContent"
      inner
      bold
      title-size="sm"
    />

    <ListWrap
      title="成长与收获："
      :list="teamReward"
      inner
      bold
      title-size="sm"
      type="ul"
    />
  </ProjectWrap>
</template>

<script setup lang="ts">
import { ref } from "vue";
import TitleDesc from "../../../components/TitleDesc/TitleDesc.vue";
import ProjectWrap from "../../../components/ProjectWrap/ProjectWrap.vue";
import ListWrap from "../../../components/ListWrap/ListWrap.vue";

const teamContent = ref([
  "对复杂功能流程图的绘制，重要需求变更留存；",
  "团队制定UI规范；明确了公共变量名，主题色值等；",
  "前端代码规范(包括ESlint、Prettier等配置，模块、组件命名、写法和其他约定)；",
  "theme 相关主题变量、normalize、mixin等；",
  "业务组件二次封装，为产品和UI提供demo示例。",
]);

const teamReward = ref([
  "团队参与感，成员获得成就感",
  "每次提交即review，互相学习",
  "更加注重反馈与用户体验",
]);
</script>

<style>
.team-build .iconfont {
  font-size: 20px !important;
  position: relative;
  top: -2px;
}
</style>
