<script setup>
  import { ref } from "vue";
  const count = ref(0);
</script>

<template>
  <main class="counter">
    <div>
        <h2> 
        The current count is... 
        </h2>
        <h1> {{ count }} </h1>
        <button class="btn-add" @click="count--"> - </button>
        <button class="btn-remove" @click="count++"> + </button>
        <button class="clear" @click="count = 0"> Clear </button>
    </div>
</main>
</template>

<style scoped>
    main {
        background-color: aliceblue;
        height:100vh;
        width:100vw;

        display: flex;
        align-items: center;
        justify-content: center;
    }

    div {
      text-align: center;
      padding: 20px;
    }
</style>