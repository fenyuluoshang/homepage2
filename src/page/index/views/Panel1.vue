<template>
  <div class="panel1">
    <!-- <div class="bg"></div> -->
    <div class="bg-phone"></div>
    <div class="banner">
      <img draggable="false" src="@/assets/20180520160438.jpeg">
    </div>
    <nav class="navs">
      <div class="icon">
        <a target="_blank" href="http://space.bilibili.com/11435676">
          <i class="iconfont icon-CN_bilibiliB"></i>
        </a>
      </div>
      <div class="icon">
        <a target="_blank" href="https://music.163.com/#/user/home?id=406210869">
          <i class="iconfont icon-CN_NetEasemusic"></i>
        </a>
      </div>
      <div class="icon">
        <a target="_blank" href="https://github.com/fenyuluoshang">
          <i class="iconfont icon-POP_GitHub"></i>
        </a>
      </div>
      <div class="line"></div>
    </nav>
    <div class="main-head">
      <h1>纷羽Shiner</h1>
      <p>死肥宅真可怕 / 沉迷ACG / 沉迷coding / 双十一生人怎么了</p>
    </div>
    <blobCard class="blob-mainpage"/>
  </div>
</template>
<script>
import blobCard from "./BlobCard.vue";
export default {
  components: {
    blobCard
  }
};
</script>
<style lang="scss" scoped>
@import "@/assets/screen.scss";

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
.navs {
  .icon {
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
  }
}

@media (min-width: $media-screen-width) {
  .bg-phone {
    display: none;
  }
  .banner {
    position: absolute;
    height: 70vh;
    width: 70%;
    top: 12vh;
    left: -20%;
    box-shadow: 5px 4px 4px rgba($color: #000000, $alpha: 0.25);
    z-index: 1;
  }
  .blob-mainpage {
    position: absolute;
    width: 35%;
    height: 30vh;
    bottom: 5vh;
    left: 42%;
    padding: 3%;
    z-index: 2;
    background-color: #97c7ff;
    box-shadow: 5px 5px 4px rgba($color: #000000, $alpha: 0.25);
  }
  .main-head {
    position: absolute;
    left: 55%;
    top: 6vh;
    max-width: 37%;
    h1 {
      color: #505050;
      font-size: 3rem;
      @media (max-width: $max-screen-width - 1px) {
        font-size: 2rem;
      }
      padding-bottom: 10px;
      font-family: "SimSun";
    }
    p {
      color: #505050;
      font-size: 2rem;
      @media (max-width: $max-screen-width - 1px) {
        font-size: 1.3rem;
      }
      font-family: "SimSun";
    }
  }
  .navs {
    position: absolute;
    right: 3vw;
    top: 40vh;
    .icon {
      padding-bottom: 16px;
    }
    .line {
      position: relative;
      height: calc(60vh - 151px);
      border-right: 2px solid #000000;
      right: 18px;
    }
  }
  .iconfont {
    font-size: 34px;
    line-height: 34px;
  }
  .icon-CN_bilibiliB {
    font-size: 39px;
  }
}
@media (max-width: $media-screen-width) {
  $banner-height: 30vh;
  .banner {
    width: 100%;
    height: $banner-height;
  }
  .bg-phone {
    width: 100%;
    position: absolute;
    top: 0;
    height: $banner-height;
    background: linear-gradient(
      to bottom,
      rgba($color: #ffffff, $alpha: 0),
      rgba($color: #ffffff, $alpha: 0.5)
    );
    z-index: 1;
  }
  .navs {
    background: #ffffff;
    height: 30px;
    .icon {
      float: left;
      width: 33.33%;
      text-align: center;
      a {
        i {
          font-size: 22px;
          line-height: 30px;
        }
      }
      .line {
        display: none;
      }
    }
  }

  .main-head {
    background-color: #fafafa;
    padding: 10px;
    h1 {
      padding-bottom: 10px;
    }
  }
  .blob-mainpage {
    padding: 10px 0;
  }
}
</style>
<style lang="scss">
@import "@/assets/screen.scss";
@media (max-width: $media-screen-width) {
  .blob-mainpage {
    h2 {
      padding-left: 15px;
    }
    .links {
      div {
        padding: 0 10px;
      }
    }
  }
}
.card {
  min-height: 60vh;
  width: 60%;
  margin: 10vh 10%;
  padding: 10vh 10%;
  background-color: rgba($color: #f0f0f0, $alpha: 0.8);
  border-radius: 15px;
  box-shadow: 7px 5px 5px rgba($color: #000000, $alpha: 0.25);
  @media (max-width: $media-screen-width) {
    width: 80%;
    min-height: 80vh;
    margin: 5vh 5%;
    padding: 5vh 5%;
  }
}
</style>
