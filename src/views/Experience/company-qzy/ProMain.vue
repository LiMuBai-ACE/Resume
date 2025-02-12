<template>
  <ProjectWrap
    class="pl-4"
    title="齐著云商城小程序"
    label="技术栈"
    :description="`一个根据年轻人喜好的服装商城，主要页面有首页，分享中心，购物车，客服聊天，个人中心这五个页面，实
现的主要功能有支付，推广，赚佣金，拼团，限时购，消息推送，海报分享等功能`"
  >
    <template #lib>
      <Button plain type="info" size="small">Taro</Button>
      <Button plain type="info" size="small">Taro-UI</Button>
      <Button plain type="info" size="small">TypeScript</Button>
      <Button plain type="info" size="small">Redux</Button>
      <Button plain type="info" size="small">WebScoket</Button>
    </template>
  </ProjectWrap>

  <ProjectWrap
    class="pl-4"
    title="齐著云商城移动端"
    label="技术栈"
    :description="`商城h5端`"
  >
    <template #lib>
      <Button plain type="info" size="small">React</Button>
      <Button plain type="info" size="small">React-Router</Button>
      <Button plain type="info" size="small">antd-mobile</Button>
      <Button plain type="info" size="small">Axios</Button>
      <Button plain type="info" size="small">WebScoket</Button>
    </template>
  </ProjectWrap>
  <ProjectWrap
    class="pl-4"
    title="齐著云商户平台"
    label="技术栈"
    :description="`多商户入驻的管理平台，主要有商品管理，订单管理，售后管理，商城管理，营销中心，会员运营，
数据中心，账号管理，公告中心，客服这些大的功能模块。商家平台管理员拥有最高级的权限，可以添加其他管理员分配不
同的用户权限，各个管理员展示不同的可操作管理信息。`"
  >
    <template #lib>
      <Button plain type="info" size="small">Vue</Button>
      <Button plain type="info" size="small">Element</Button>
      <Button plain type="info" size="small">Vue-Router</Button>
      <Button plain type="info" size="small">Vuex</Button>
      <Button plain type="info" size="small">Axios</Button>
      <Button plain type="info" size="small">Echarts</Button>
      <Button plain type="info" size="small">WebScoket</Button>
    </template>
  </ProjectWrap>
</template>

<script setup lang="ts">
import ProjectWrap from "../../../components/ProjectWrap/ProjectWrap.vue";
import { Button } from "fri-element-plus";
</script>
