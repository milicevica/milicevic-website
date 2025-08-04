<script lang="ts" setup>
const route = useRoute();
const slug = route.params.slug || [];

const { data: page } = await useAsyncData(() =>
  queryCollection("content")
    .path(`/${slug}`)
    .first(),
);
</script>

<template>
  <ContentRenderer v-if="page" :value="page" />
  <div v-else>
    Blog post not found.
  </div>
</template>
