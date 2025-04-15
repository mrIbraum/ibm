<script setup lang="ts">
    import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';
    import { faPhone } from '@fortawesome/free-solid-svg-icons';

    
</script>

<template>
    <div class="max-w-[1320px] min-w-[1320px] flex items-center justify-between absolute z-1 pt-4 mt-6">
        <div class="text-white text-[3rem] font-bold"><span class="text-blue-600">O</span>.</div>
        <ul class="border border-[#181818] border-2 h-[50px] w-[50%] rounded-full px-4 py-1 flex items-center justify-between bg-[linear-gradient(45deg,#000000,#000000)] shadow-lg">
            <li class="text-zinc-200">Home</li>
            <li class="text-zinc-400">About</li>
            <li class="text-zinc-400">Skills</li>
            <li class="text-zinc-400">Projects</li>
            <li class="text-zinc-400">Parcours</li>
            <li class="text-zinc-400">Services</li>
            <li class="text-zinc-400">Contact</li>
        </ul>
        <div class="flex items-center gap-2">
            <!-- <RouterLink :to="''" :color="'white'" class="group h-[45px] w-[45px] text-xl border border-2 border-zinc-500 rounded-full flex items-center justify-center shadow-lg duration-150 hover:text-zinc-600 hover:bg-[linear-gradient(45deg,#242424,#000000)] duration-150">
                <FontAwesomeIcon :icon="faPhone" class="group-hover:text-white text-zinc-500 duration-150" />
            </RouterLink> -->
            <div class="w-[50px] h-[50px] rounded-full flex items-center justify-center text-white bg-[linear-gradient(45deg,#242424,#000000)]">
                CV
            </div>
        </div>
    </div>
</template>

<style>
    
</style>