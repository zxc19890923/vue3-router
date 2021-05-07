<template>
  <div class="contain">
    <div id="nav">
      <div style="height: 20px"></div>
      <router-link to="/user" active-class="active">
        <div class="navBtn">用户</div>
      </router-link>
      <router-link to="/test" active-class="active">
        <div class="navBtn">测试</div>
      </router-link>
    </div>
    <div class="navChild">
      <router-view/>
    </div>
  </div>
</template>
<style lang="scss" scoped>
  .contain {
    display: flex;
    flex-direction: row;
    height: 100%;
    width: 100%;
    #nav {
      width: 60px;
      height: 100%;
      text-align: center;
      background: #444;
      color: #fff;
      .navBtn {
        padding: 20px 0;
        color: #ccc;
        background: #333;
        flex: 1;
      }
      .active .navBtn {
        color: #fff;
        background: #000;
      }
    }
    .navChild {
      flex: 1;
    }
  }
</style>
