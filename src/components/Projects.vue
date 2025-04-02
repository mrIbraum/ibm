<script setup lang="ts">
import { ref } from 'vue';

    const projectsField = ref(
        [
            {
                libel: "Dashboard",
                projects: [
                    {
                        imagePath: "",
                        title: "ESGIS Presencia",
                        description: "A web app for course managment"
                    },
                    {
                        imagePath: "",
                        title: "APM",
                        description: "A web app for manage parking"
                    }
                ]
            },
            {
                libel: "Simple CRUD App",
                projects: [
                    {
                        imagePath: "",
                        title: "Book managment",
                        description: "A web app for book managment"
                    },
                    {
                        imagePath: "",
                        title: "GAPE",
                        description: "A web app for staff managment"
                    }
                ]
            },
            {
                libel: "Mobile App",
                projects: [
                    {
                        imagePath: "",
                        title: "MindMaze",
                        description: "A quiz game with TRIVIA api"
                    }
                ]
            }
        ]
    );

</script>

<template>
    <div class="w-full min-h-[100vh] flex items-center justify-between relative overflow-hidden">
        <div class="bg-[url(../../public/pattern-skills.svg)] bg-cover bg-no-repeat opacity-10 -z-0 absolute w-full min-h-[100vh] top-0 left-0 rignt-0 bottom-0"></div>

        <div class="absolute h-[400px] w-full bg-[linear-gradient(180deg,var(--color),transparent)] rounded-full blur-[100px] left-[0%] top-[-150px] opacity-[0.35]"></div>
        <div class="absolute h-[400px] w-full bg-[linear-gradient(0deg,var(--color),transparent)] rounded-full blur-[140px] left-[0%] bottom-[0px] opacity-[0.25]"></div>

        <div class="w-full min-h-[100vh] pt-[25px] px-[75px] flex flex-col items-center justify-start z-1">
            <div class="bg-[linear-gradient(90deg,var(--color),white)] bg-clip-text text-transparent text-[2.5vw] font-bold z-1">Projects</div>
            <div class="flex items-start justify-center flex-wrap w-full mt-[30px] gap-5">
                <template v-for="projects in projectsField" :key="projects.libel">
                    <div class="flex flex-col">
                        <div class="w-full text-start text-[1.2vw] mb-1 font-bold text-zinc-600">{{ projects.libel }}</div>
                        <div class="flex gap-3">
                            <template v-for="project in projects.projects">
                                <div @click="" class="relative clickable hover:scale-[1.01] duration-150 w-[300px] h-[250px] p-3 flex flex-col gap-3 rounded bg-[linear-gradient(45deg,#1D1D1D,#090909,#090909,#1D1D1D)]">
                                    <div class="w-full h-full bg-[linear-gradient(45deg,var(--color))] opacity-[0.1] absolute top-0 left-0 z-0 rounded"></div>
                                    <div class="clickable w-full h-[150px] border border-zinc-800 rounded overflow-hidden">
                                        <img :src="project.imagePath" alt="project images" class="object-cover object-center">
                                    </div>
                                    <div class="clickable text-xl text-zinc-400 flex flex-col gap-2">
                                        <div class="text-xl">{{ project.title }}</div>
                                        <p class="text-[1rem] text-zinc-600 w-full whitespace-normal overflow-hidden text-ellipsis">
                                            {{ project.description }}
                                        </p>
                                    </div>
                                </div>
                            </template>
                        </div>
                    </div>
                </template>
            </div>
        </div>
        <div class="h-[200px] w-full bg-[linear-gradient(180deg,#000000,rgba(0,0,0,0))] absolute top-0 z-0"></div>
        <div class="h-[100px] w-full bg-[linear-gradient(0deg,#000000,rgba(0,0,0,0))] absolute bottom-0 z-0"></div>
    </div>
</template>

<style scoped>
    
</style>