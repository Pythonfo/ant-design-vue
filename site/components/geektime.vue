<template>
  <div id="geektime" v-show="visible">
    <a
      href="https://time.geekbang.org/course/intro/163?code=KHKYcoBU6vZa8nMglg7AWfDxxi3BWrz9INAzAY3umPk%3D"
      target="_blank"
    >
      <img
        width="170"
        alt="Vue 实战教程"
        src="https://cdn.nlark.com/yuque/0/2019/jpeg/87084/1562230861353-assets/web-upload/2fab2df7-5cc9-4791-b344-a97da29eb400.jpeg"
      >
    </a>
    <div v-if="isMobile" class="close" @click="visible=false">
      <a-icon type="close"></a-icon>
    </div>
  </div>
</template>

<script>
export default {
  props: ['isMobile'],
  data() {
    return {
      visible: true
    }
  }
};
</script>

<style lang="less" scoped>
  #geektime {
    position: fixed;
    bottom: 15px;
    right: 15px;
    .close {
      position: absolute;
      text-align: center;
      top: -8px;
      right: -8px;
      font-size: 16px;
      padding: 15px;
      color: #6e3041;
    }
  }
</style>

