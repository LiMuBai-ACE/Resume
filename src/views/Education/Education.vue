<template>
  <Section title="教育经历" anchor="Education" icon="peixunjiaoyu">
    <RowContent
      label="西安电子科技大学（信息科学与技术）"
      :label-bold="true"
      text="2020年9月——2023年1月"
      align="right"
      :is-wrap="true"
    />
    <RowContent
      label="平顶山工业职业技术学院（建筑工程技术）"
      :label-bold="true"
      text="2016年9月——2019年6月"
      align="right"
      :is-wrap="true"
    />
  </Section>
</template>

<script setup lang="ts">
import Section from "../../components/Layouts/Section.vue";
import RowContent from "../../components/RowContent/RowContent.vue";
</script>
