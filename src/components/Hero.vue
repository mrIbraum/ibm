<script setup lang="ts">
    import gsap from 'gsap';
    import { onMounted, ref } from 'vue';
    import Social from './Social.vue';
    import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';
    import { faGithub, faWhatsapp, faLinkedin, faTelegram } from '@fortawesome/free-brands-svg-icons';

    const icons = ref(
        [
            {
                name: faGithub,
                href: "",
                libel: "github",
                color: "hover:bg-[#181717]",
                shadow: "hover:shadow-[0_10px_20px_1px_grey]"
            },
            {
                name: faLinkedin,
                href: "",
                libel: "linkedin",
                color: "hover:bg-[#0A66C2]",
                shadow: "hover:shadow-[0_10px_20px_1px_#0A66C2]"
            },
            {
                name: faWhatsapp,
                href: "",
                libel: "whatsapp",
                color: "hover:bg-[#25D366]",
                shadow: "hover:shadow-[0_10px_20px_1px_#25D366]"
            },
            {
                name: faTelegram,
                href: "",
                libel: "telegram",
                color: "hover:bg-[#0088CC]",
                shadow: "hover:shadow-[0_10px_20px_1px_#0088CC]"
            }
        ]
    );

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
    <div class="max-w-[1320px] min-h-[100vh] flex items-center justify-between relative pt-[50px]">
        <img src="@/assets/img/pattern.svg" alt="" class="pattern w-[200rem] absolute right-[-35%] z-0">
        <div class="absolute h-[300px] w-[300px]   bg-[linear-gradient(135deg,var(--color),transparent)] rounded-full blur-[150px] right-0 top-0"></div>
        <div class="absolute h-[600px] w-[600px]   bg-[linear-gradient(-45deg,var(--color),transparent)] rounded-full blur-[200px] left-[40%] bottom-[0%] opacity-50"></div>
        <div class="text-box min-h-[100vh] w-[60%] flex flex-col items-start justify-center gap-5">
            <div class="md:text-[3vw] text-white font-bold leading-[80px]"><span class="text-[2.25vw]">Hello, I'm KONDO Ibrahim</span> <br><span id="" class="fullstack text-[3.8vw] text-transparent bg-clip-text font-extrabold  bg-[linear-gradient(90deg,var(--color),white)] leading-[75px] scale-y-[1.1]">Web Developper <br> & Data Visualization</span></div>
            <div class="text-xl text-white w-[80%]">Je transforme les idées en projets concrets avec une touche de créativité.
                Entre rigueur et imagination, je cherche toujours le bon équilibre.</div>
            <div class="flex items-center gap-4 pt-6">
                <div class="">
                    <router-link to="" class="hover:bg-blue-600 hover:text-white duration-200 hover:shadow-[0_10px_20px_1px_var(--color)] px-[40px] py-[15px] text-blue-600 border border-blue-600 border-2 text-[1rem] rounded-full bg-transparent">Download CV</router-link>
                </div>
                <div class="text-2xl flex gap-2">
                    <RouterLink :to="icon.href"  v-for="icon in icons" :key="icon.libel" :color="'white'" :href="icon.href" class="h-[45px] w-[45px] text-xl border border-2 border-blue-600 rounded-full flex items-center justify-center shadow-lg duration-150"  :class="[icon.color, icon.shadow]">
                        <Social :color="''">
                            <FontAwesomeIcon :icon="icon.name" :style="{color: '#fff',}" />
                        </Social>
                    </RouterLink>
                </div>
                <!-- <router-link to="" class="px-[50px] py-[10px] text-white text-xl rounded-full bg-transparente border border-2 border-zinc-600 text-zinc-500">Contact me </router-link> -->
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