<template>
  <div class="result-fail">
    <t-icon class="result-fail-icon" name="error-circle" />
    <div class="result-fail-title">创建失败</div>
    <div class="result-fail-describe">抱歉，您的项目创建失败，企业微信联系检查创建者权限，或返回修改。</div>
    <div>
      <t-button @click="() => this.$router.push('/dashboard/base')">返回修改</t-button>
      <t-button theme="default" @click="() => this.$router.push('/dashboard/base')">返回首页</t-button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'result-fail',
};
</script>

<style lang="less" scoped>
@import '@/style/variables.less';

.result-fail {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 75vh;

  &-icon {
    font-size: 72px;
    color: @text-color-secondary;
  }

  &-title {
    margin-top: 28px;
    font-size: 20px;
    color: @text-color-primary;
    text-align: center;
    line-height: 28px;
    font-weight: 500;
  }

  &-describe {
    margin: 8px 0 32px;
    font-size: 14px;
    color: @text-color-secondary;
    line-height: 22px;
  }
}
</style>
