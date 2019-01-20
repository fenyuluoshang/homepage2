<template>
  <div class="home">
    <div class="firstpanel panel">
      <div class="banner">
        <img draggable="false" src="@/assets/20180520160438.jpeg">
      </div>
      <nav class="line">
        <i class="iconfont icon-CN_bilibiliB"></i>
        <i class="iconfont icon-CN_NetEasemusic"></i>
        <i class="iconfont icon-POP_GitHub"></i>
        <i class="iconfont icon-POP_mail"></i>
      </nav>
      <blobCard class="blob-mainpage"/>
      <div class="main-head">
        <h1>纷羽Shiner</h1>
        <p>死肥宅真可怕 / 沉迷ACG / 沉迷coding / 双十一生人怎么了</p>
      </div>
    </div>
    <div class="panel"></div>
  </div>
</template>

<script>
import blobCard from "./BlobCard.vue";
export default {
  name: "home",
  components: {
    blobCard
  }
};
</script>
<style lang="scss" scoped>
@import "@/assets/screen.scss";

@media (min-width: $max-screen-width) {
  .panel {
    height: 100vh;
  }
  .banner {
    position: absolute;
    height: 70vh;
    width: 70%;
    top: 12vh;
    right: 55%;
    box-shadow: 4px 4px 4px rgba($color: #000000, $alpha: 0.25);
    z-index: 1;
  }
  .banner > img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  .banner > div {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  .blob-mainpage {
    position: absolute;
    width: 40%;
    height: 30vh;
    bottom: 5vh;
    left: 40%;
    padding: 3%;
    z-index: 2;
    background-color: #97c7ff;
    box-shadow: 5px 5px 4px rgba($color: #000000, $alpha: 0.25);
  }
  .main-head {
    position: absolute;
    left: 50%;
    top: 6vh;
    max-width: 42%;
    h1 {
      color: #505050;
      font-size: 3rem;
      font-family: "SimSun";
    }
    p {
      color: #505050;
      font-size: 2rem;
      font-family: "SimSun";
    }
  }
  .icon {
    width: 50px;
    height: 50px;
    background-size: 100% 100%;
    background-repeat: no-repeat;
  }
}
</style>
