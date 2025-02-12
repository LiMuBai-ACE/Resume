<template>
  <Section anchor="Experience" title="工作经历" icon="gongzuoxinxi">
    <CompanyBZ />
    <div class="divide flex my-3"></div>
    <CompanyCPMC />
    <div class="divide flex my-3"></div>
    <CompanyQzy />
  </Section>
</template>

<script setup lang="ts">
import Section from "../../components/Layouts/Section.vue";
import CompanyBZ from "./company-bz/index.vue";
import CompanyCPMC from "./company-cpmc/index.vue";
import CompanyQzy from "./company-qzy/index.vue";
</script>
