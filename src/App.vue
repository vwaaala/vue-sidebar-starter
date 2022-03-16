<script setup>

import SideBar from "./components/SideBar.vue";
</script>

<template>
  <div class="app">
    <SideBar/>
    <router-view/>
  </div>

</template>

<style lang="scss">
:root {
  --primary: hsl(171, 100%, 41%);
  --secondary: hsl(48, 100%, 67%);
  --darkcyan: #008b8b;
  --black: hsl(0, 0%, 4%);
  --danger: hsl(348, 100%, 61%);

  --white: hsl(0, 0%, 100%);
  --greyLight-1: #ebf2fc;
  --greyLight-2: #d5ddf3;
  --greyLight-3: #bec8e4;
  --greyDark: #5b657a;
  --sidebar-width: 300px;
}
*, *::before, *::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Crimson Pro', serif;
}
body{
  background: var(--greyDark);
  color: var(--primary);
}
button {
  cursor: pointer;
  appearance: none;
  border: none;
  outline: none;
  background: none;
}

.app{
  display: flex;

  main{
    flex: 1 1 0;
    padding: 2rem;
    @media (max-width: 768px) {
      padding-left: 6rem;
    }
  }
}
</style>
