<template>
  <div>
    <header>
      <div class="header">
        <div class="logo">MusicMosaic</div>
        <div class="menu-btn">
          <ul>
            <li>
              <router-link to="/home">Home</router-link>
              <router-link to="/about">About</router-link>
            </li>
          </ul>
        </div>
      </div>
    </header>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header {
  .header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    .logo {
    }
    .menu-btn {
    }
  }
}
</style>
