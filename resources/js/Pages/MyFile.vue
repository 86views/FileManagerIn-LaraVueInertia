<template>
    <AuthenticatedLayout>
        {{ $page.url }}
    </AuthenticatedLayout>
</template>
<script setup>
import AuthenticatedLayout from "@/Layouts/AuthenticatedLayout.vue";
import { Head } from "@inertiajs/vue3";
</script>

<style scoped></style>
