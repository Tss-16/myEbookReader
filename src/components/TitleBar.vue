<template>
  <transition name="slide-down">
      <div class="title-wrapper" v-show="ifTitleAndMenuShow">
        <h3 class="title">TFH's ebook</h3>
      </div>
    </transition>
</template>

<script>
export default {
  props: {
    ifTitleAndMenuShow: {
      type: Boolean,
      default: false
    }
  }
}

</script>

<style lang='scss' scoped>
@import '../assets/styles/global';
.title-wrapper {
    position: absolute;
    top: 0;
    left: 0;
    z-index: 101;
    display: flex;
    width: 100%;
    height: px2rem(48);
    background: white;
    box-shadow: 0 px2rem(8) px2rem(8) rgba(0, 0, 0, .15);
    justify-content: center;

    .title {
      text-align: center;
      font-size: px2rem(20);
      font-weight: 600;
      line-height: px2rem(48);

    }
  }

</style>
