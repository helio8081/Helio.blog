<template>
    <a class="inline-flex items-center justify-center px-3 py-2 mt-2 mr-2 rounded-md bg-gray-50 transition-colors decoration-none 
        hover:text-white dark:bg-gray-50/10" :class="item.class" :href="item.link" target="_blank"
        v-for="(item, index) in socialLists" :key="index">
        <div>
            <i :class="item.icon"></i>
        </div>
        <div class="text-sm ml-1" v-if="item.text">{{ item.text }}</div>
    </a>
    <div>

    </div>
</template>

<script setup>
import { reactive } from 'vue';


const socialLists = reactive([
    {
        text: 'Github',
        link: 'https://github.com/helio8081',
        icon: 'ri-github-fill',
        class: 'hover:bg-gray-700 dark:hover:bg-white dark:hover:text-gray-900'
    }, {
        text: '',
        link: 'https://www.figma.com/@Helio8081',
        icon: 'ri-figma-line',
        class: 'hover:bg-[#f7c104]'
    }, {
        text: '',
        link: 'https://space.bilibili.com/177837736',
        icon: 'ri-bilibili-fill',
        class: 'hover:bg-[#fb7299]'
    },
])

</script>