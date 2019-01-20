<template>
  <div class="home">
    <panel1 class="panel"/>
    <!-- <div class="panel" :style="{backgroundColor:'#f0f0f0'}"></div> -->
  </div>
</template>

<script>
import panel1 from "./Panel1.vue";
export default {
  name: "home",
  components: {
    panel1
  }
};
</script>
<style lang="scss" scoped>
.panel {
  height: 100vh;
}
</style>
