<template>
    <nav class="font-mono">
        <ul class="flex space-x-4">
            <li>
                <NuxtLink to="/" class="link">Main</NuxtLink>
            </li>
            <li>
                <NuxtLink to="/about" class="link">About</NuxtLink>
            </li>
            <li>
                <NuxtLink to="/project" class="link">Project</NuxtLink>
            </li>
        </ul>
    </nav>
</template>

<script setup>
useHead({
    titleTemplate: '%s - Furkan Turgut',

})
</script>

<style scoped>
.link {
    @apply p-1 hover:bg-gray-200
}
</style>