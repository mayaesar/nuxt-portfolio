<script lang="ts" setup>
import type { NavigationMenuItem } from "@nuxt/ui";

const items = ref<NavigationMenuItem[][]>([
  [
    {
      label: "Home",
      icon: "lucide:house",
      to: "/",
    },
    {
      label: "About me",
      icon: "lucide:smile",
      to: "/",
    },
    {
      label: "Projects",
      icon: "lucide:file-code-2",
      to: "/",
      active: true,
    },
    {
      label: "Contact",
      icon: "lucide:messages-square",
      to: "/",
      active: true,
    },
  ],
  [
    {
      label: "GitHub",
      icon: "i-simple-icons-github",
      to: "https://github.com/mayaesar",
      target: "_blank",
    },
    {
      label: "Resume",
      icon: "lucide:download",
      to: "/resume.pdf",
      target: "_blank",
      download: "resume.pdf",
    },
  ],
]);
</script>

<template>
  <div>
    <UNavigationMenu color="neutral" :items="items" class="w-full" />
  </div>
</template>
