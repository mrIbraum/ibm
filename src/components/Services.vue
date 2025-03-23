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
    <div class="w-full min-h-[100vh] flex items-center justify-between relative overflow-hidden">
        <div class="w-full min-h-[100vh] pt-[25px] px-[75px] flex flex-col items-start justify-start">
            <div class="text-white text-[2.5vw] font-bold z-1">Services</div>
        </div>
        <div class="h-[200px] w-full bg-[linear-gradient(180deg,#000000,rgba(0,0,0,0))] absolute top-0 z-0"></div>
        <div class="h-[100px] w-full bg-[linear-gradient(0deg,#242424,rgba(0,0,0,0))] absolute bottom-0 z-0"></div>
    </div>
</template>

<style scoped>

</style>