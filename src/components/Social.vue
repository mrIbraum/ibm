<script setup lang="ts">
    interface props {
        color: string;
    };

    const myProps = defineProps<props>();

    const color = "text-"+myProps.color;
</script>

<template>
    <div class="h-[25px] w-[25px] text-2xl" :class="color">
        <slot></slot>
    </div>
</template>

<style scoped>
    
</style>