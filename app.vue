<template>
  <main>
      <h1>Web Class</h1>
      <h2>second class</h2>
      <div class="slot-area">
          <slot class="slot-area"/>
      </div>
      <menu>
          <li>
              <NuxtLink to="/">Home</NuxtLink>
          </li>
          <li2>
              <a href="https://github.com/yejinnnnnhi/demo03.git">My first class</a>
          </li2>
      </menu>
  </main>
</template>

<style lang="scss">
    main {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr 1fr;
        grid-auto-rows: auto;
        h1 {
            grid-column: 3 / 4; 
            grid-row: 5 / 6;
        }
        h2 {
            grid-column: 3 / 4;
            grid-row: 7 / 8;
        }
        menu {
            grid-column: 3 / 4;
            grid-row: 6 / 7;
        }
        .slot-area {
            grid-column: 1 / 4;
        }
    
    }
</style>
