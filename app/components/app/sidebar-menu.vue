<script setup>
const navItems = [
  { text: "About", link: "/" },
  { text: "Blog", link: "/blog" },
  { text: "Random", link: "/random" },
];
</script>

<template>
  <aside class="flex flex-col items-start text-sm text-gray-400 md:w-1/4">
    <nav class="space-y-2">
      <NuxtLink
        v-for="item in navItems"
        :key="item.text"
        :to="item.link"
        class="block"
        exact-active-class="text-emerald-500"
      >
        {{ item.text }}
      </NuxtLink>
    </nav>
  </aside>
</template>
