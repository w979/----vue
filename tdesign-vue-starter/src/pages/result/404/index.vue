<template>
  <result title="404 Not Found" tip="抱歉，您访问的页面不存在" type="404">
    <t-button @click="() => $router.push('/dashboard/base')">返回首页</t-button>
  </result>
</template>

<script>
import result from '@/components/result/index.vue';

export default {
  name: 'result-404',
  components: { result },
};
</script>
