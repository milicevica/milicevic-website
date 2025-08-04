<template>
  <div class="max-w-4xl w-full flex flex-col md:flex-row gap-8">
    <!-- Sidebar -->
    <aside class="flex flex-col items-start text-sm text-gray-400 md:w-1/4">
      <div class="text-emerald-500 text-xl font-bold mb-4">
        AM
      </div>
      <nav class="space-y-2">
        <a href="#" class="text-emerald-500 block">About</a>
        <a href="#" class="hover:text-white block">Blog</a>
        <a href="#" class="hover:text-white block">Random</a>
      </nav>
    </aside>

    <!-- Main Content -->
    <main class="md:w-3/4 text-sm space-y-4">
      <h1 class="text-white font-semibold uppercase">
        Aleksandar Milicevic
      </h1>

      <p>I'm a developer living in Belgrade, Serbia.</p>

      <p>Currently I spend most of my time working as a Software Engineer at <a href="#" class="text-emerald-500 underline">Deluxe</a>, on a print on demand ecommerce project.</p>

      <p>
        In my free time I play racing simulations. I currently play F1 2025. 🏎️
      </p>

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
</template>
