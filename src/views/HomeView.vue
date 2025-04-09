<template>
    <div class="w-full min-h-[100vh] flex flex-col items-center relative bg-[linear-gradient(0deg,black,black,black)] overflow-hidden">
        <NavBar />
        <Hero />
        <About />
        <Skills />
        <Projects />
        <Parcours />
        <Services />
        <!-- <div v-if="show" @click="hidePopup" class="fixed w-full h-[100vh] bg-black opacity-[0.75] z-2"></div>
        <div v-if="show" class="fixed w-[60%] h-[300px] bg-[linear-gradient(30deg,#1D1D1D,#090909,#1D1D1D,#090909,#1D1D1D)]  rounded-[10px] shadow-lg translate-[-50%] top-[50%] left-[50%] z-3">
            <div class="w-full h-full relative p-2 flex flex-col items-start justify-start">
                <div class="w-full h-full bg-[linear-gradient(45deg,var(--color))] opacity-[0.1] absolute top-0 left-0 rounded-[10px] z-3"></div>
                <div class="text-3xl text-white bg-clip-text font-bold">Under construction</div>
                <div class="text-2xl text-white bg-clip-text font-bold pt-8">
                    <ul>
                        <li> - Not responsive</li>
                        <li> - Not finished</li>
                    </ul>
                </div>
                <div class="absolute z-4 right-2 top-1 text-3xl text-white clickable" @click="hidePopup">
                    <FontAwesomeIcon :icon="faCircleXmark" />
                </div>
            </div>
        </div> -->
    </div>
</template>

<script setup lang="ts">
    import NavBar from "../components/NavBar.vue";
    import Hero from "../components/Hero.vue";
    import About from "../components/About.vue";
    import Skills from "../components/Skills.vue";
    import Projects from "../components/Projects.vue";
    import Parcours from "../components/Parcours.vue";
    import Services from "../components/Services.vue";
    import { ref } from "vue";
    import { FontAwesomeIcon } from "@fortawesome/vue-fontawesome";
    import { faCircleXmark } from "@fortawesome/free-solid-svg-icons";

    const show = ref(true);

    const hidePopup = () => {
        show.value = false;
    };

</script>

<style scoped>
    
</style>