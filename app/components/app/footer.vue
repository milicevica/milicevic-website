<script setup>
const socials = [
  { name: "mail", link: "mailto:hi@milicevid.dev" },
  { name: "brand-twitter", link: "https://x.com/milicev1ca" },
  { name: "brand-github", link: "https://github.com/milicevica" },
  { name: "brand-linkedin", link: "https://www.linkedin.com/in/milicevica/" },
];
</script>

<template>
  <footer class="flex flex-row  items-center justify-between pt-8 text-xs text-gray-500">
    <p>© {{ new Date().getFullYear() }} Aleksandar Milicevic.</p>
    <div class="flex space-x-2 mt-2 text-lg text-gray-500">
      <a
        v-for="social in socials"
        :key="social.name"
        :href="social.link"
        target="_blank"
      >
        <Icon :name="`tabler:${social.name}`" />
      </a>
    </div>
  </footer>
</template>
