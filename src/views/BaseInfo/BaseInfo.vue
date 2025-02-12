<template>
  <Section title="基本信息" icon="mingpian">
    <RowContent label="姓名" text="李帅兵" />
    <RowContent label="学历" text="本科（非全日制）" />
    <RowContent label="工作经验" text="六年" />
    <RowContent label="所在地" text="上海市" />

    <RowContent label="求职意向" text="前端工程师" />
  </Section>
</template>

<script setup lang="ts">
import Section from "../../components/Layouts/Section.vue";
import RowContent from "../../components/RowContent/RowContent.vue";
</script>
