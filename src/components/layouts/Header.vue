<template>
  <div>
    <header>
      <div class="header">
        <div class="logo">MusicMosaic</div>
        <div class="menu-btn">
          <ul>
            <li>
              <router-link to="/">Home</router-link>
              <router-link to="/about">About</router-link>
            </li>
          </ul>
        </div>
      </div>
      <video
        class="bg-video"
        loop=""
        autoplay="true"
        muted
        src="@/assets/video.mp4"
        type="video/mp4"
      ></video>
    </header>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
header {
  .header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    .logo {
      font-family: "Quicksand";
      font-size: 30px;
      color: antiquewhite;
    }
    .menu-btn {
      ul {
        li {
          a {
            font-family: "Quicksand";
            font-size: 20px;
            color: antiquewhite;
          }
        }
      }
    }
  }
}
.bg-video {
  position: absolute;
  width: 100%;
  height: 100%;
  left: 0%;
  top: 0%;
  z-index: -1;
  object-fit: cover;
  filter: brightness(50%) blur(2px);
}
</style>
