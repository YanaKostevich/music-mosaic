<template>
  <div class="home">
    <Header />
    <video
      class="bg-video"
      loop=""
      autoplay="true"
      muted
      src="../assets/video.mp4"
      type="video/mp4"
    ></video>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from "@/components/layouts/Header.vue";

console.log(Header);
export default {
  components: {
    Header,
  },
};
</script>

<style lang="scss">
.bg-video {
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0;
  left: 0;
  z-index: -1;
  object-fit: cover;
  filter: brightness(50%) blur(2px);
}
</style>
