<template>
  <div>
    <h2>Blob / 个人博客</h2>
    <a target="_blank" href class="links" v-for="blobhref in bloblist" :key="blobhref.id">
      <div>{{blobhref.tittle}}</div>
    </a>
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
h2 {
  padding-bottom: 17px;
  font-family: "SimHei";
}
a {
  color: #000000;
  text-decoration: none;
  outline: none;
  :hover {
    color: #000000;
    text-decoration: none;
    outline: none;
  }
}
.links {
  display: inline;
  text-decoration: none;
  div {
    margin-bottom: 8px;
    padding: 5px 0;
    font-family: "SimSun";
    transition: 0.2s all;
  }
  :hover {
    opacity: 1;
    transform: translateY(-3px);
    background: rgba($color: #f0f0f0, $alpha: 0.2);
  }
}
</style>