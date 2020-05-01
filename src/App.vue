<template>
  <div id="app" style="--webkit-app-region: drag" class="font-sans flex min-h-screen">
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>-->
    <Sidebar />
    <router-view />
  </div>
</template>

<script>
import Sidebar from "./components/Sidebar";

export default {
  name: "App",
  components: {
    Sidebar
  }
};
</script>

<style>
</style>