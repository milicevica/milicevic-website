<script setup>
import { NuxtLink } from "#components";

const { data: posts } = await useAsyncData(() => queryCollection("content").all());
</script>

<template>
  <div>
    <h1 class="text-sm space-y-4">
      Welcome to my blog!
    </h1>

    <p class="text-sm space-y-4">
      Here, I'll be writing about anything that interests me — whether it's tech, racing simulation games, or whatever else captures my curiosity.
    </p>

    <ul class="list  rounded-box shadow-md">
      <li class="pt-4 pb-2 text-xs opacity-60 tracking-wide">
        Posts:
      </li>

      <li
        v-for="(post, index) in posts"
        :key="post.id"
        class="list-row"
      >
        <div class="text-4xl font-thin opacity-30 tabular-nums">
          {{ String(index + 1).padStart(2, '0') }}
        </div>
        <!-- <div><img class="size-10 rounded-box" src="https://img.daisyui.com/images/profile/demo/1@94.webp"></div> -->
        <div class="list-col-grow">
          <NuxtLink :to="`/blog${post.path}`">
            <div>Aleksandar Milicevic</div>
            <div class="text-xs uppercase font-semibold opacity-60">
              {{ post.title }}
            </div>
          </NuxtLink>
        </div>
        <NuxtLink :to="`/blog${post.path}`" class="btn btn-square btn-ghost">
          <Icon name="tabler:arrow-big-right" size="24" />
        </NuxtLink>
      </li>
    </ul>
  </div>
</template>
