<script setup lang="ts">
    import gsap from 'gsap';
    import { onMounted } from 'vue';
    import Social from './Social.vue';

    onMounted(() => {
        gsap.from(".pattern", { rotation: 0, x: 600, duration: 1 });
        gsap.to(".pattern", { rotation: 0, x: 0, duration: 1 });
        gsap.from(".text-box", { rotation: 0, x: -800, duration: 1 });
        gsap.to(".text-box", { rotation: 0, x: 0, duration: 1 });
        var split = new SplitText(".fullstack", {type: "chars"});
        gsap.from(split.chars, {
            duration: 5, 
            y: 100, 
            autoAlpha: 0, 
            stagger: 0.05
        });
    });
</script>

<template>
    <div class="w-full min-h-[100vh] px-[75px] flex items-center justify-between relative overflow-hidden">
        <img src="../../public/pattern.svg" alt="" class="pattern w-[200rem] absolute right-[-35%] z-0">
        <div class="text-box min-h-[100vh] flex flex-col items-start justify-center gap-2">
            <div class="text-small text-zinc-300">Welcome !</div>
            <div class="md:text-[3vw] text-white font-bold">Hello, I'm KONDO Ibrahim <br>A <span id="" class="fullstack text-zinc-600">fullstack developper</span> & <br> junior in <span class="text-zinc-400">data visualization</span>.</div>
            <div class="text-xl text-white">Open to work, just download my cv and contact me.</div>
            <div class="flex gap-4 pt-6">
                <router-link to="" class="hover:bg-white hover:text-black duration-200 hover:shadow-[0_10px_20px_1px_rgba(255,255,255,0.3)] px-[50px] py-[10px] text-white text-xl rounded-full bg-zinc-700">Download CV</router-link>
                <router-link to="" class="px-[50px] py-[10px] text-white text-xl rounded-full bg-transparente border border-2 border-zinc-600 text-zinc-500">Contact me </router-link>
            </div>
            <div class="flex items-center justify-start gap-4">
                <template >
                    <Social :color="'red-100'" v-for="i in 4"  :key="i">
                        {{ i }}
                    </Social>
                </template>
            </div>
        </div>
        <div class="h-[100px] w-full bg-[linear-gradient(0deg,#000000,rgba(0,0,0,0))] absolute bottom-0"></div>
    </div>
</template>

<style scoped>
    .text-stroked {
        -webkit-text-stroke-width: 0.5px;
        -webkit-text-stroke-color: white;
        color: transparent;
    }

    .fullstack {
        display: inline-block;
        transform-style: preserve-3d;
        perspective: 800px;
        /* backface-visibility: hidden; */
    }
</style>