<template>
    <div class="w-full min-h-[100vh] flex flex-col items-center relative bg-[linear-gradient(0deg,black,black,black)] overflow-hidden">
        <NavBar />
        <Hero />
        <About />
        <Skills />
        <Projects />
        <Parcours />
        <Services />
        <div v-show="show" class="fixed w-full h-[100vh] bg-blue-600"></div>
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

    const show = ref(true);

    const hidePopup = () => {
        show.value = false;
    };

</script>

<style scoped>
    
</style>