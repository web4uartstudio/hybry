<template>
  <div
    class="overlay w-screen h-screen fixed top-0 left-0 z-10"
    @click="showHideSidebar"
    @wheel.prevent
    @touchmove.prevent
    @scroll.prevent
  ></div>
</template>

<script>
export default {
  methods: {
    showHideSidebar() {
      this.$store.commit("showHideSidebar");
    },
  },
};
</script>

<style lang="scss" scoped>
.overlay {
  background: rgba(94, 88, 214, 0.5);
}
</style>
