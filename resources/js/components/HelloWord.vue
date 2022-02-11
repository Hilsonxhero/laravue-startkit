<template>
    <div class="grid items-center h-screen">
        <div>
            <button
                class="bg-gray-400 py-4 px-6 rounded-lg text-white flex"
                @click="increment"
            >
                {{ state.count }}
            </button>
        </div>
    </div>
</template>
<script setup>
import { ref, reactive } from "vue";

const state = reactive({ count: 0 });

const increment = () => {
    state.count++;
};
</script>
<style></style>
