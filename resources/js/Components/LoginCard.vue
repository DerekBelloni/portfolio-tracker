<template>
    <Card
     pt:root:class="border border-gray-300 border-solid rounded-lg"
     pt:title:class="flex justify-center my-6"
     >
        <template #title>
            <span class="text-2xl text-gray-700">Login</span>
        </template>
        <template #content>
            <div class="m-12">
                <FloatLabel variant="on">
                    <InputText id="username" type="text" pt:root:class="border border-solid rounded-lg bg-gray-50"></InputText>
                    <label for="username">Username</label>
                </FloatLabel>
            </div>
        </template>
    </Card>
</template>

<script setup>
import Card from 'primevue/card';
import InputText from 'primevue/inputtext';
import FloatLabel from 'primevue/floatlabel';
</script>