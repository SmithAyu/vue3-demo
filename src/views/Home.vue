<template>
  <div class="home">
    <div class="topnav">Topnav</div>
    <div class="content">
      <aside>边栏</aside>
      <main>内容</main>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
// @ is an alias to /src

export default defineComponent({
  components: {},
});
</script>
<style lang="scss" scoped>
.home {
  display: flex;
  flex-direction: column;
  height: 100vh;
  .topnav {
    background: #00a4ff;
  }
  .content {
    display: flex;
    flex-grow: 1;
    > aside {
      background: #115600;
      width: 200px;
    }
    > main {
      background: lightgreen;
      flex-grow: 1;
    }
  }
}
</style>
