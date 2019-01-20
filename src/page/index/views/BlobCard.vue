<template>
  <div>
    <h2>Blob / 个人博客</h2>
    <div v-for="blobhref in bloblist" :key="blobhref.id">
      <a>{{blobhref.tittle}}</a>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      bloblist: [
        {
          id: 1,
          tittle: "Python3 与 node-sass不兼容问题和解决方案"
        },
        {
          id: 2,
          tittle: "第十届蓝桥杯参赛总结"
        },
        {
          id: 3,
          tittle: "教职工晚会炸了3台服务器的事故总结"
        }
      ]
    };
  }
};
</script>
<style lang="scss" scoped>
</style>