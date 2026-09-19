<script setup lang="ts">
    import {ref} from "vue";

    const count = ref(0);

    const add = () => {
        count.value++;
    }

</script>

<template>
    <h3>Your current count is:</h3>
    <p> {{ count }}</p>
    <div>
        <button @click="add">Add</button>
    </div>
</template>

<style>

</style>