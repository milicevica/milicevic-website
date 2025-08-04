<template>
  <aside class="flex flex-col items-start text-sm text-gray-400 md:w-1/4">
    <nav class="space-y-2">
      <NuxtLink
        to="/"
        class="block"
        exact-active-class="text-emerald-500"
      >
        About
      </NuxtLink>
      <NuxtLink
        to="/blog"
        class="hover:text-white block"
        exact-active-class="text-emerald-500"
      >
        Blog
      </NuxtLink>
      <NuxtLink
        to="/random"
        class="hover:text-white block"
        exact-active-class="text-emerald-500"
      >
        Random
      </NuxtLink>
    </nav>
  </aside>
</template>
