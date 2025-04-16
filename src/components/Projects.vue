<template>
  <h2 class="flex items-center mt-14 mb-4 font-semibold text-3xl">
    <span class="title flex-1">Projects</span>
    <div class="opacity-50 ml-2 hover:opacity-100 transition-opacity cursor-pointer">
      <i class=" m-2 ri-arrow-right-up-line"></i>
    </div>
  </h2>
  <div class="grid gap-4 grid-cols-1 sm:grid-cols-2">
    <a class="px-4 py-3 rounded-md bg-gray-50 transition-colors decoration-none hover:bg-gray-100 dark:bg-gray-50/10 dark:hover:bg-gray-50/20"
      :href="item.link" target="_blank" v-for="(item, index) in ProjectList" :key="index">
      <div class="flex h-full items-center justify-center">
        <div class="mr-4 text-4xl">
          <div :class="item.icon"></div>
        </div>
        <div class="flex-1">
          <div class="font-medium leading-relaxed">{{ item.name }}</div>
          <div class="opacity-50 font-normal text-sm">{{ item.desc }}</div>
        </div>
      </div>
    </a>
  </div>
</template>

<script setup>
import { reactive } from 'vue';

const ProjectList = reactive([
  {
    name: 'Smart Retail',
    desc: 'Smart retail backend management',
    link: 'https://retailtest.mobxcx.com/',
    icon: 'i-fluent-emoji-flat:shopping-bags',
  },
  {
    name: 'Retail Mall',
    desc: 'Retail mall mini program',
    link: '#',
    icon: 'i-fluent-emoji-flat:feather',
  },
  {
    name: 'Retail Assistant',
    desc: 'Smart retail assistant mini program',
    link: '#',
    icon: 'i-fluent-emoji-flat:small-airplane',
  },
  {
    name: 'Local Lifestyle Shopping',
    desc: 'Local life shopping backend management',
    link: 'https://retailtest.mobxcx.com/',
    icon: 'i-fluent-emoji-flat:cactus',
  },
])
</script>
