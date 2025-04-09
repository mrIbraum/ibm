<script setup lang="ts">

    const parcours = [
        {
            id: 1,
            logo: "",
            title: "Architecture Logiciel",
            year: "2022 - present"
        },
        {
            id: 1,
            logo: "",
            title: "Stage En Support Services Vas.",
            year: "2022 - present"
        },
        {
            id: 1,
            logo: "",
            title: "Student On DataCamp Plateform.",
            year: "2022 - present"
        }
    ];
</script>

<template>
    <div class="w-full min-h-[100vh] flex items-center justify-between relative overflow-hidden">
        <img src="../assets/img/manifesto-extra.tracks.png" alt="" class="absolute w-[500px] left-[-100px] opacity-[0.75]">
        <img src="../assets/img/manifesto-extra.tracks.png" alt="" class="absolute w-[500px] bottom-[-200px] right-[-100px] opacity-[0.5] rotate-[180deg]">
        <div class="w-full min-h-[100vh] pt-[25px] px-[75px] gap-7 flex flex-col items-center justify-start">
            <div class="bg-[linear-gradient(90deg,var(--color),white)] bg-clip-text text-transparent text-[2.5vw] font-bold z-1">Parcours</div>
            <div class="w-[80%] min-h-[300px] text-white text-center z-1">
                <div v-for="parcour in parcours" class="flex items-center justify-start gap-6 w-full px-5 py-[4rem] bg-stone-100 mb-6 rounded relative bg-[linear-gradient(45deg,#1D1D1D,#090909,#1D1D1D,#090909,#1D1D1D)] hover:bg-[linear-gradient(45deg,#242424,#090909,#1D1D1D)] duration-300">
                    <div class="text-3xl font-bold text-slate-500">{{ parcour.title }}</div>
                    <div class="w-full h-full bg-[linear-gradient(45deg,var(--color))] opacity-[0.1] absolute top-0 left-0 z-0"></div>
                </div>
            </div>
        </div>
        <div class="h-[200px] w-full bg-[linear-gradient(180deg,#000000,rgba(0,0,0,0))] absolute top-0 z-0"></div>
        <div class="h-[100px] w-full bg-[linear-gradient(0deg,#000000,rgba(0,0,0,0))] absolute bottom-0 z-0"></div>
    </div>
</template>

<style scoped>

</style>