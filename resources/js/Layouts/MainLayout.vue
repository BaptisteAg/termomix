<script setup lang="ts">
import {Head, Link} from '@inertiajs/vue3';
import ApplicationLogo from "@/Components/ApplicationLogo.vue";

</script>
<template>
    <div class="min-h-screen bg-slate-900 text-white">
        <header>
            <div class="py-3 bg-slate-950 text-white">
                <nav class="flex items-center justify-between gap-8 px-8 text-xl">
                    <div>
                        <Link :href="route('index')">
                            <ApplicationLogo
                            />
                        </Link>
                    </div>
                    <div class="hover:text-slate-400">
                        <Link
                            v-if="$page.props.auth.user"
                            :href="route('dashboard')">
                            Dashboard
                        </Link>
                        <Link
                            v-else
                            :href="route('login')">
                            Login
                        </Link>
                    </div>
                </nav>
            </div>
        </header>
        <main>
            <slot/>
        </main>
    </div>
</template>
