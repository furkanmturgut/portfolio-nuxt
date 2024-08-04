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
    link: [
        {
            rel: 'preconnect',
            href: 'https://fonts.googleapis.com'
        },
        {
            rel: 'stylesheet',
            href: 'https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap',
            crossorigin: ''
        }
    ]
})
</script>

<style scoped>
.link {
    @apply p-1 hover:bg-gray-200
}

body{
        font-family: 'Poppins';
    }
</style>