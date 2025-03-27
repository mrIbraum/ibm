<script setup lang="ts">
import { ref } from 'vue';

    const projectsField = ref(
        [
            {
                libel: "Landing",
                projects: [
                    {
                        imagePath: "",
                        title: "",
                        description: ""
                    },
                    {
                        imagePath: "",
                        title: "Landing pages",
                        description: "nubvubzubvuizbvuevibzrivbuizebvuzbvuzbvuzebvuzbviubzibziebvuziebvuezbvizvbizebviuzbevizbjdcjqncjoncvaevobaevoibaovbaubvuabvuiebvuieavbiaebviyebvivih"
                    }
                ]
            }
        ]
    );

</script>

<template>
    <div class="w-full min-h-[100vh] flex items-center justify-between relative overflow-hidden">
        <!-- <div class="bg-[url(../../public/pattern-skills.svg)] bg-cover bg-no-repeat opacity-10 -z-0 absolute w-full min-h-[100vh] top-0 left-0 rignt-0 bottom-0"></div> -->
        <div class="w-full min-h-[100vh] pt-[25px] px-[75px] flex flex-col items-center justify-start z-1">
            <div class="text-white text-[2.5vw] font-bold z-1">Projects</div>
            <div class="flex items-start justify-start flex-wrap w-full mt-[30px] gap-3">
                <template v-for="projects in projectsField" :key="projects.libel">
                    <div class="w-full text-start text-[1vw] mb-3 text-zinc-700 border border-0 border-b-1 border-dashed">{{ projects.libel }}</div>
                    <template v-for="project in projects.projects">
                        <div @click="" class="clickable hover:scale-[1.01] duration-150 w-[18%] h-[250px] p-3 flex flex-col gap-3 rounded bg-[linear-gradient(45deg,#1D1D1D,#090909,#090909,#1D1D1D)] border border-2 border-zinc-800 shadow-[0_0_10px_1px_rgba(255,255,255,0.09)]">
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
                </template>
            </div>
        </div>
        <div class="h-[200px] w-full bg-[linear-gradient(180deg,#000000,rgba(0,0,0,0))] absolute top-0 z-0"></div>
        <div class="h-[100px] w-full bg-[linear-gradient(0deg,#000000,rgba(0,0,0,0))] absolute bottom-0 z-0"></div>
    </div>
</template>

<style scoped>
    
</style>