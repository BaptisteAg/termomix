<script setup lang="ts">
import {Head, Link} from '@inertiajs/vue3';
import ApplicationLogo from "@/Components/ApplicationLogo.vue";

defineProps<{}>();

</script>

<template>
    <Head title="VuttVuuutt"/>
    <div class="min-h-screen bg-slate-900 text-white">
        <application-logo></application-logo>
        <header class="p-4">
            <h1 class="text-3xl font-bold">VuttVuuutt</h1>
        </header>
        <section class="p-4">
            <h2 class="text-2xl mb-4">Recommended for You</h2>
            <!-- Ajouter un composant de liste de films ici -->
        </section>
        <section class="p-4">
            <h2 class="text-2xl mb-4">New Releases</h2>
            <!-- Ajouter un composant de liste de films ici -->
        </section>
        <!-- Vous pouvez ajouter d'autres sections ici -->
    </div>
</template>
