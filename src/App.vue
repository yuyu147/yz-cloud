<template>
  <div id="app">
    <div id="nav">
      <router-link to="/"></router-link>
    </div>
    <router-view />
  </div>
</template>



<style>
@import url("../src/assets/base.less");
@import url("../src/assets/normalize.css");
#app {
  font-family: "Microsoft YaHei", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #464459;
}
#nav {
  /* padding: 30px; */
}
</style>
