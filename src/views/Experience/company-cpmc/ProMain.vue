<template>
  <ProjectWrap
    class="pl-4"
    title="UCMT学习平台"
    label="技术栈"
    :description="`该学习平台专为中大型企业设计，提供员工在线培训功能，满足企业在新员工培训、在线考试和内部培训等方面的需求。平台主要模块包括精选课程、直播、考试、学习任务、公司资讯和平台推荐等。此外，平台与钉钉办公系统深度融合，融入工作场景，提供全新高效的企业培训方式。`"
  >
    <template #lib>
      <Button plain type="info" size="small">React</Button>
      <Button plain type="info" size="small">Ant Design</Button>
      <Button plain type="info" size="small">Umi</Button>
      <Button plain type="info" size="small">Canvas</Button>
      <Button plain type="info" size="small">Echarts</Button>
    </template>

    <ListWrap title="主要贡献：" :list="mainList" inner bold />
  </ProjectWrap>
  <ProjectWrap
    class="pl-4"
    title="学员报名小程序"
    label="技术栈"
    :description="`学员报名系统主要用于学员报名使用，销售在后台创建学院项目后，分享小程序码给学员，学员通过扫码进入小程序，
并进行信息填报。当学员信息在后台通过审核后，通过短信和小程序通知的形式，发送面试通知和预录取通知。 `"
  >
    <template #lib>
      <Button plain type="info" size="small">Taro</Button>
      <Button plain type="info" size="small">Taro-UI</Button>
      <Button plain type="info" size="small">Dva</Button>
      <Button plain type="info" size="small">Sass</Button>
      <Button plain type="info" size="small">Axios</Button>
    </template>
  </ProjectWrap>
  <ProjectWrap
    class="pl-4"
    title="UCMT后台管理"
    label="技术栈"
    :description="`UCMT后台管理系统主要用于用户端各大功能模块内容的管理主要功能模块有：数据可视化报表、课程管理、讲师管理、
考试管理、咨询管理、培训管理、直播管理、员工管理、系统设置等。其中采用数字化展示员工（学员）的学习情况，用于
分析各类课程的学习情况，改良课程质量，为学员创造更好的课程体验。  `"
  >
    <template #lib>
      <Button plain type="info" size="small">React</Button>
      <Button plain type="info" size="small">Ant Design</Button>
      <Button plain type="info" size="small">Umi</Button>
      <Button plain type="info" size="small">Echarts</Button>
    </template>
  </ProjectWrap>
</template>

<script setup lang="ts">
import { ref } from "vue";
import ProjectWrap from "../../../components/ProjectWrap/ProjectWrap.vue";
import ListWrap from "../../../components/ListWrap/ListWrap.vue";
import { Button } from "fri-element-plus";

const mainList = ref([
  "准确理解产品需求和设计交互原型，设计出合理的代码功能模块；",
  "采用aliPlayer对课程视频播放的的处理，可根据后台配置进行用户是否可以快进，可拖动，同时记录视频播放进度，以便用户下观看；",
  "采用动态路由方案，便于企业对不使用或者还未开始使用的模块进行动态管理；",
  "用户分享海报的绘制。",
]);
</script>
