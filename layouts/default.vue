<template>
    <main>
        <h1>Title</h1>
        <div class="slot-area">
            <slot class="slot-area" />
        </div>
        <menu>
            <li>
                <NuxtLink to="/">Home</NuxtLink>
            </li>
            <li>
                <NuxtLink to="/about">About</NuxtLink>
            </li>
        </menu>
    </main>
</template>

<script>

</script>

<style lang="scss">
    main {
        display: grid;

        grid-template-columns: 1fr 1fr 1fr 1fr;
        grid-auto-rows: auto;

        h1 {
            grid-column: 4 / 5;
            grid-row: 1 / 2;
        }

        .slot-area {
            grid-column: 1 / 4;
        }

        menu {
            grid-column: 4 / 5;
            grid-row: 2 / 3;
        }
    }
</style>