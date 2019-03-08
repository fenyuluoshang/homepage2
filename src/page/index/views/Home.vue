<template>
  <div class="home">
    <panel1/>
    <panel2/>
  </div>
</template>

<script>
import panel1 from "./Panel1.vue";
import panel2 from "./Panel2.vue";
export default {
  name: "home",
  components: {
    panel1,
    panel2
  }
};
</script>
<style lang="scss">
@import "@/assets/screen.scss";
.panel1 {
  padding-bottom: 10vh;
  @media (min-width: $media-screen-width) {
    min-height: 100vh;
  }
}
</style>
