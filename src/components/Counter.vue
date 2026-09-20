<script setup lang="ts">
    import {ref, computed} from "vue";

    const count = ref(0);
    const doubleCount = computed(() => count.value * 2);

    function add() {
        count.value++;
    }

    function remove() {
        count.value--;
    }

</script>

<template>
    <h3>Your current count is:</h3>
    <p> Single counter: {{ count }}</p>
    <p> Double counter: {{ doubleCount }}</p>
    <div>
        <button @click="add">Count up</button>
        <button @click="remove">Count down</button>
    </div>
</template>

<style>

</style>