<script setup>
    
</script>

<template>
    <div class="w-full min-h-[100vh] flex items-center justify-center relative overflow-hidden">
        <div class="max-w-[1320px] h-[100vh] flex items-center justify-end">
            <div class="w-[50%] h-full flex flex-col items-start justify-center pl-5 gap-4">
                <div class="text-[2.5vw] font-bold bg-[linear-gradient(90deg,var(--color),white)] bg-clip-text text-transparent">About Me</div>
                <div class="text-[1.25vw] text-zinc-400 pr-[75px]">
                    Curious, rigorous, and solution-oriented, I see development as a powerful lever for connecting ideas to real-world applications. Through this portfolio, I share projects that reflect my vision: clean code, user-focused interfaces, and systems capable of adapting to real-world needs.
                    <br>
                    <br>
                    My career path revolves around web development, intelligent automation, and data analysis. I work on projects where technology serves efficiency, exploring areas such as IoT, APIs, and backend architectures. My goal: to learn quickly, build accurately, and contribute to robust, useful, and sustainable solutions.
                </div>
                <router-link to="" class="hover:bg-blue-600 hover:text-white duration-200 hover:shadow-[0_10px_20px_1px_var(--color)] px-[40px] py-[15px] text-blue-600 border border-blue-600 border-2 text-[1rem] rounded-full bg-transparent">Download CV</router-link>
            </div>
        </div>
        <div class="absolute h-[200px] w-[200px]   bg-[linear-gradient(135deg,var(--color),transparent)] rounded-full blur-[150px] right-0 top-0"></div>
        <div class="absolute h-[300px] w-[300px]   bg-[linear-gradient(135deg,var(--color),transparent)] rounded-full blur-[200px] right-[10%] bottom-0"></div>
        <div class="absolute h-[600px] w-[600px]   bg-[linear-gradient(-45deg,var(--color),transparent)] rounded-full blur-[200px] left-[0%] bottom-[0%] opacity-50"></div>
        <img src="../../public/pattern-about.svg" alt="" class="w-[75vw] absolute left-[-30%]">
        <div class="h-[100px] w-full bg-[linear-gradient(180deg,#000000,rgba(0,0,0,0))] absolute top-0"></div>
        <div class="h-[100px] w-full bg-[linear-gradient(0deg,#000000,rgba(0,0,0,0))] absolute bottom-0"></div>
    </div>
</template>

<style scoped>
    
</style>