<template>
  <div class="no-result">
    <div class="no-result-icon"></div>
    <p class="no-result-text">{{title}}</p>
  </div>
</template>

<script>
  export default {
    name: 'no-result',
    props: {
      title: {
        type: String,
        default: ''
      }
    }
  }
</script>

<style scoped lang="less">
  @import "../../common/styles/_vars.less";
  @import "../../common/styles/_mixin.less";

  .no-result{
    text-align: center;
    .no-result-icon{
      width: 86px;
      height: 90px;
      margin: 0 auto;
      .bg-image('../../base/no-result/no-result');
      background-size: 86px 90px;
    }
    .no-result-text{
      margin-top: 30px;
      font-size: @font-size-medium;
      color: @color-text-d;
    }
  }
</style>
