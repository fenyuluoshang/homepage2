<template>
  <div>
    <h2>Blob / 个人博客</h2>
    <a target="_blank" :href="blobhref.href" class="links" v-for="blobhref in bloblist" :key="blobhref.id">
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
          tittle: "typescript类型推导",
          href: 'https://blog.fenyu.club/typescript/typescript%E7%B1%BB%E5%9E%8B%E6%8E%A8%E5%AF%BC.html'
        },
        {
          id: 2,
          tittle: "跨页面的消息传输",
          href: 'https://blog.fenyu.club/study/daily/%E8%B7%A8%E9%A1%B5%E9%9D%A2%E7%9A%84%E6%B6%88%E6%81%AF%E4%BC%A0%E8%BE%93.html'
        },
        {
          id: 3,
          tittle: "浏览插件开发的一点记录",
          href: 'https://blog.fenyu.club/study/Vue/%E6%B5%8F%E8%A7%88%E5%99%A8%E6%8F%92%E4%BB%B6%E5%BC%80%E5%8F%91%E6%80%BB%E7%BB%93.html'
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