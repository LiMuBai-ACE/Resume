<template>
  <Section title="专业技能" anchor="Skill" icon="zhuanyezhishijineng">
    <ListWrap title="前端" :list="feList" bold />

    <ListWrap title="其他" :list="otherList" bold type="ul" />
  </Section>
</template>

<script setup lang="ts">
import { ref } from "vue";
import Section from "../../components/Layouts/Section.vue";
import ListWrap from "../../components/ListWrap/ListWrap.vue";

const feList = ref([
  "精通 HTML、CSS，具备扎实的前端基础，善于处理主流浏览器的兼容性问题；",
  "熟练掌握 JavaScript、TypeScript 及 ES6+ 语法，拥有丰富的 React + TS + JS 开发经验；",
  "熟悉 Vue 及其相关技术栈，能够快速适应并上手项目开发；",
  "深入理解前端开发全流程，从代码编写到上线部署，对协同开发、分支管理、项目配置等有丰富的实践经验；",
  "熟悉 Webpack、Vite 等前端构建工具，掌握其核心原理和优化策略。",
]);

const otherList = ref([
  "熟悉 Node.js 及其常用模块，具备一定的后端开发能力；",
  "了解 Golang 的基础语法，并对其开发流程和项目架构有一定了解；",
  "了解 Linux 常用命令，能够独立完成项目部署；",
  "善于利用搜索引擎和 AI 工具提升开发效率，坚持高效工作原则。",
]);
</script>
