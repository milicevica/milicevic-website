<template>
  <div class="min-h-screen flex items-center justify-center px-4 py-12">
    <div class="max-w-4xl w-full flex flex-col md:flex-row gap-8">
      <aside class="flex flex-col items-start text-sm text-gray-400 md:w-1/4">
        <div class="text-emerald-500 text-3xl font-bold mb-4">
          AM
        </div>
        <nav class="space-y-2">
          <a href="#" class="text-emerald-500 block">About</a>
          <a href="#" class="hover:text-white block">Blog</a>
          <a href="#" class="hover:text-white block">Random</a>
        </nav>
      </aside>

      <main class="space-y-4">
        <h1 class="text-white font-semibold uppercase text-3xl">
          Aleksandar Milicevic
        </h1>

        <slot />

        <footer class="flex flex-row items-center justify-between pt-8 text-xs text-gray-500">
          <p>© 2025 Aleksandar Milicevic.</p>
          <div class="flex space-x-2 mt-2 text-lg text-gray-500">
            <a href="#"><Icon name="tabler:mail" /></a>
            <a href="#"><Icon name="tabler:brand-twitter" /></a>
            <a href="#"><Icon name="tabler:brand-github" /></a>
            <a href="#"><Icon name="tabler:brand-linkedin" /></a>
          </div>
        </footer>
      </main>
    </div>
  </div>
</template>
