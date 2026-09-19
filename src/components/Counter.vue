<script setup lang="ts">
    import {ref, computed} from "vue";

    const count = ref(0);
    const doubleCount = computed(() => count.value * 2);

    const add = () => {
        count.value++;
    }

    const remove = () => {
        count.value--;
    }

</script>

<template>
    <h3>Your current count is:</h3>
    <p> Single counter: {{ count }}</p>
    <p> Souble counter: {{ doubleCount }}</p>
    <div>
        <button @click="add">Add</button>
        <button @click="remove">Remove</button>
    </div>
</template>

<style>

</style>