<template>
  <div class="flex flex-col items-center p-12">
    <div class="w-full max-w-4xl flex flex-col flex-1 mt-36">
      <AppThemeToggle />
      <AppNavBar />

      <main class="flex-1 flex flex-col md:flex-row gap-4 mt-16">
        <AppSidebarMenu />

        <div class="flex flex-col md:w-3/4">
          <div class="min-h-[150px]">
            <slot />
          </div>

          <AppFooter />
        </div>
      </main>
    </div>
  </div>
</template>
