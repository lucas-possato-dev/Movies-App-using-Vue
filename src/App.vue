<script setup>
import { RouterView, RouterLink } from "vue-router";
</script>

<template>
  <header>
    <RouterLink to="/">
      <h1><span>Crimson</span>Movies</h1>
    </RouterLink>
  </header>
  <main>
    <RouterView />
  </main>
</template>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Fira Sans", sans-serif;

  &::selection {
    background: transparentize(#42b883, 0.5);
  }
}

body {
  background-color: #333;
}

a {
  text-decoration: none;
}

header {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 10px 16px;
  background-color: #222;
  box-shadow: 0px 0px 6px rgba(0, 0, 0, 0.1);
}

h1 {
  color: #fff;
  font-size: 28px;

  span {
    color: crimson;
  }
}
</style>
