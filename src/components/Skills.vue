<script setup lang="ts">
import { faBitbucket, faBootstrap, faCss3Alt, faFigma, faGit, faGithub, faGitlab, faHtml5, faJs, faLaravel, faNodeJs, faPhp, faPython, faVuejs } from '@fortawesome/free-brands-svg-icons';
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';

    
</script>

<template>
    <div class="w-full min-h-[100vh] flex items-center justify-between relative overflow-hidden">
        <div class="w-full min-h-[100vh] px-[75px] z-1 pt-[50px]">
            <div class="text-white text-[2.5vw] font-bold">Skills</div>
            <div class="min-h-[80vh] w-full flex justify-between gap-2 flex-wrap mt-[25px]">
                <div class="w-[20%] grow-1 text-zinc-500 p-3 rounded bg-[linear-gradient(45deg,#1D1D1D,#090909,#1D1D1D,#090909,#1D1D1D)] hover:bg-[linear-gradient(45deg,#242424,#090909,#1D1D1D)] duration-200">
                    <div class=" text-zinc-600 border border-0 border-b-1 border-zinc-800">frontend</div>
                    <div class="mt-3 w-full flex flex-wrap gap-0">
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <FontAwesomeIcon :icon="faHtml5" class="text-[1.8vw] hover:text-orange-500 shadow-lg hover:shadow-[0_10px_10px_1px_text-orange-500]"/>
                        </div>
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <FontAwesomeIcon :icon="faCss3Alt" class="text-[1.8vw] hover:text-blue-500"/>
                        </div>
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <FontAwesomeIcon :icon="faJs" class="text-[1.8vw] hover:text-yellow-500"/>
                        </div>
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <FontAwesomeIcon :icon="faVuejs" class="text-[1.8vw]  hover:text-green-500"/>
                        </div>
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <div class=" hover:text-cyan-500 text-[1vw]">Tailwind</div>
                        </div>
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <FontAwesomeIcon :icon="faBootstrap" class="text-[1.8vw] hover:text-purple-500"/>
                        </div>
                    </div>
                </div>
                <div class="w-[20%] grow-1 text-zinc-500 p-3 rounded bg-[linear-gradient(45deg,#1D1D1D,#090909,#1D1D1D,#090909,#1D1D1D)] hover:bg-[linear-gradient(45deg,#242424,#090909,#1D1D1D)] duration-200">
                    <div class=" text-zinc-600 border border-0 border-b-1 border-zinc-800">backend</div>
                    <div class="mt-3 w-full flex flex-wrap gap-0">
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <FontAwesomeIcon :icon="faPhp" class="text-[1.8vw] hover:text-purple-300"/>
                        </div>
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <FontAwesomeIcon :icon="faNodeJs" class="text-[1.8vw] hover:text-green-600"/>
                        </div>
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <FontAwesomeIcon :icon="faLaravel" class="text-[1.8vw] hover:text-red-500"/>
                        </div>
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <div class="hover:text-yellow-400 text-[1vw]">Express JS</div>
                        </div>
                    </div>
                    <div class="mt-3 text-zinc-600 border border-0 border-b-1 border-zinc-800">data Science</div>
                    <div class="mt-3 w-full flex flex-wrap gap-0">
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <FontAwesomeIcon :icon="faPython" class="text-[1.8vw] hover:text-yellow-400"/>
                        </div>
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <div class="text-[1vw]">Panda</div>
                        </div>
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <div class="text-[1vw]">Numpy</div>
                        </div>
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <div class="text-[1vw]">Matplotlib</div>
                        </div>
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <div class="text-[1vw]">Sql</div>
                        </div>
                    </div>
                </div>
                <div class="w-[20%] grow-1 text-zinc-500 p-3 rounded bg-[linear-gradient(45deg,#1D1D1D,#090909,#1D1D1D,#090909,#1D1D1D)] hover:bg-[linear-gradient(45deg,#242424,#090909,#1D1D1D)] duration-200">
                    <div class=" text-zinc-600 border border-0 border-b-1 border-zinc-800">tools & versionning</div>
                    <div class="mt-3 w-full flex flex-wrap gap-0">
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <FontAwesomeIcon :icon="faGithub" class="text-[1.8vw] hover:text-stone-400"/>
                        </div>
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <FontAwesomeIcon :icon="faGitlab" class="text-[1.8vw] hover:text-orange-400"/>
                        </div>
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <FontAwesomeIcon :icon="faBitbucket" class="text-[1.8vw] hover:text-blue-500"/>
                        </div>
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <FontAwesomeIcon :icon="faGit" class="text-3xl hover:text-orange-400"/>
                        </div>
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <div class="hover:text-blue-400 text-[1vw]">Vs Code</div>
                        </div>
                    </div>
                </div>
                <div class="w-[20%] grow-1 text-zinc-500 p-3 rounded bg-[linear-gradient(45deg,#1D1D1D,#090909,#1D1D1D,#090909,#1D1D1D)] hover:bg-[linear-gradient(45deg,#242424,#090909,#1D1D1D)] duration-200">
                    <div class=" text-zinc-600 border border-0 border-b-1 border-zinc-800">databases</div>
                    <div class="mt-3 w-full flex flex-wrap gap-0">
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <div class=" hover:text-sky-900 text-[1vw]">Mysql</div>
                        </div>
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <div class=" hover:text-green-900 text-[1vw]">MongoDB</div>
                        </div>
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <div class=" hover:text-sky-900 text-[1vw]">PostgreSQL</div>
                        </div>
                    </div>
                    <div class="mt-3 text-zinc-600 border border-0 border-b-1 border-zinc-800">others</div>
                    <div class="mt-3 w-full flex flex-wrap gap-0">
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <FontAwesomeIcon :icon="faFigma" class="text-3xl hover:text-pink-400"/>
                        </div>
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <div class=" hover:text-blue-900 text-[1vw]">Photoshop</div>
                        </div>
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <div class=" hover:text-orange-900 text-[1vw]">Illustrator</div>
                        </div>
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <div class=" hover:text-sky-900 text-[1vw]">Vercel</div>
                        </div>
                        <div class="w-[calc(100%/3)] h-[75px] flex items-center justify-center">
                            <div class=" hover:text-sky-900 text-[1vw]">Netlify</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="h-[200px] w-full bg-[linear-gradient(180deg,#000000,rgba(0,0,0,0))] absolute top-0 z-0"></div>
        <div class="h-[100px] w-full bg-[linear-gradient(0deg,#000000,rgba(0,0,0,0))] absolute bottom-0 z-0"></div>
    </div>
</template>

<style scoped>
    
</style>