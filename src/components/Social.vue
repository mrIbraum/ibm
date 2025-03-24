<script setup lang="ts">
    import { ref } from 'vue';

    const textColor = ref("");
    const borderColor = ref("");
    const bgColor = ref("");

    interface props {
        color: string;
    };

    const myProps = defineProps<props>();

    textColor.value = "text-"+myProps.color;
    borderColor.value = "border-"+myProps.color;
    bgColor.value = "bg-"+myProps.color;
</script>

<template>
    <div class="flex items-center justify-center" :class="textColor+' '+borderColor+' '+bgColor">
        <slot></slot>
    </div>
</template>

<style scoped>
    
</style>