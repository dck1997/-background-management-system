<template>
  <div class="background">
    <div class="dashboard-container">
      <div class="dashboard-text">WELCOME,{{ name }}!!!</div>
    </div>
  </div>
</template>

<script>
import { mapGetters } from 'vuex'

export default {
  name: 'Dashboard',
  computed: {
    ...mapGetters([
      'name'
    ])
  }

}
</script>

<style lang="scss" scoped>
.dashboard {
  &-container {
    margin: 30px;
  }
  &-text {
    font-size: 30px;
    line-height: 46px;
    color:blue;

  }
}
.background {
    // width: 100%;
    // height: 100%;
    // /**宽高100%是为了图片铺满屏幕 */
    // z-index: -1;
    // position: absolute;
    background:url("../../assets/home.jpg");
    width:100%;			//大小设置为100%
    height:100%;			//大小设置为100%
    position:fixed;
    background-size:100% 100%;
}

</style>
