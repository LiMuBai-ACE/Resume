<template>
  <ProjectWrap
    class="pl-4"
    title="Coach官网、SW官网、马歇尔官网等"
    description="以上项目基于成熟B端系统能力打造了一款定制化C端开发平台，旨在为全球消费者提供高端、流畅且安全的线上购物体验，集成了产品展示与管理、促销营销、购物车与订单处理以及用户认证与个性化推荐等功能，支持详细的产品描述、高清图片展示和多维度筛选，同时根据大数据分析向用户推荐，以便快速找到心仪单品；在技术实现上，采用当下流行的Next.js框架，利用其服务端渲染（SSR）和静态生成（SSG）优势显著提升首屏加载速度和SEO效果，同时借助其自带的文件系统路由机制免去手动配置，并兼具React生态系统的所有功能。"
  >
    <template #lib>
      <Button plain type="info" size="small">Next.js</Button>
      <Button plain type="info" size="small">TypeScript</Button>
      <Button plain type="info" size="small">ahooks</Button>
      <Button plain type="info" size="small">Axios</Button>
    </template>
    <ListWrap title="主要贡献：" :list="adminList" inner bold />

    <ListWrap title="项目难点：" :list="hardList" inner bold />
  </ProjectWrap>
</template>

<script setup lang="ts">
import { ref } from "vue";
import ProjectWrap from "../../../components/ProjectWrap/ProjectWrap.vue";
import ListWrap from "../../../components/ListWrap/ListWrap.vue";
import { Button } from "fri-element-plus";

const adminList = ref([
  "精确还原设计稿并采用响应式设计：严格按照设计稿进行页面开发，确保在不同设备和屏幕尺寸下，网站均能良好呈现，提升了移动端用户的访问体验；",
  "实现流畅的交互界面和动画效果：开发了用户友好的交互界面，并引入流畅的动画效果，增强了用户在浏览和购买过程中的体验，提高了用户满意度和粘性；",
  "开发核心功能模块：负责官网首页、商品列表、商品详情、购物车、订单等关键功能的开发，确保各模块功能完善且用户体验良好；",
  "优化页面性能：通过代码拆分、资源压缩、懒加载等技术手段，提升了页面加载速度，确保用户能够快速访问和浏览网站内容；",
  "数据埋点：完成了埋码工作，为运营团队提供了可靠的数据支持，助力其进行数据分析和决策。",
]);

const hardList = ref([
  "商品列表中的广告插入：根据后台配置，在搜索结果和导航后的商品列表中插入广告。根据广告图片的尺寸，对商品列表进行填充，并适配不同的屏幕尺寸，确保广告与商品列表的布局协调一致；",
  "穿搭模块的瀑布流布局：采用瀑布流布局方案渲染穿搭模块。获取图片元素和文字部分的尺寸，实现高低错落的展示效果，增强页面的视觉层次感；",
  "达人展示的视频播放优化：在达人展示功能中，主要以视频形式展示现有商品。为保证用户体验，默认展示视频封面，当用户点击播放时，动态创建 video 标签播放视频，确保当前页面仅有一个视频在播放。",
]);
</script>
