<template>
  <div class="pxb">
    <div class="pxb" @click="$router.go(-1)"></div>
    <div class="panelx ms-depth-16">
      <slot></slot>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
export default {
  name: "BottomPanel",
  components: {}
};
</script>
<style lang="css" scoped>
.panelx {
  background-color: rgba(255, 255, 255, 0.7);
  backdrop-filter: blur(10px);
  position: fixed;
  width: 100%;
  bottom: 0;
  border-radius: 2rem 2rem 0 0;
  padding: 1rem;
  padding-top: 0.5rem;
  box-sizing: border-box;
  z-index: 10200;
  overflow: visible;
  max-height: 80%;
}
.pxb {
  z-index: 10000;
  position: fixed;
  width: 100%;
  height: 100%;
}
</style>
