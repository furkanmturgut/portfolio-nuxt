<template>
    <div class="container mx-auto max-w-2xl">
        <header class="flex justify-between items-center mt-5">
           <div class="flex items-center space-x-12">
            <div>
                <NuxtLink to="/" class="text-xl font-semibold p-2 hover:bg-gray-500">Furkan Turgut</NuxtLink>
            </div>

            <Menu />
           </div>
           <ColorModeSelector />
        </header>

        <main class="p-2 mt-10">
            <slot></slot>
        </main>

    </div>
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

<style>
body {
    font-family: 'Poppins';
}

body{
    @apply bg-white dark:bg-gray-900 text-gray-700 dark:text-gray-300
}
</style>