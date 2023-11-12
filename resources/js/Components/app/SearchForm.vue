<template>
    <form class="w-[1000px] h-[80px] flex items-center">
        <div>
            <InputLabel for="name" value="Name" />

            <TextInput
                id="search"
                type="text"
                class="block w-full mr-2"
                v-model="form.search"
                placeholder="Search for Files and Folder"
                autocomplete="search"
            />

            <InputError class="mt-2" :message="form.errors.search" />
        </div>
    </form>
</template>

<script setup>
// imports
import GuestLayout from "@/Layouts/GuestLayout.vue";
import InputError from "@/Components/InputError.vue";
import InputLabel from "@/Components/InputLabel.vue";
import PrimaryButton from "@/Components/PrimaryButton.vue";
import TextInput from "@/Components/TextInput.vue";
import { Head, Link, useForm } from "@inertiajs/vue3";

// Uses

const form = useForm({
    search: "",
});
</script>

<style scoped></style>
