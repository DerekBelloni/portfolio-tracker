<template>
    <Card
     pt:root:class="border border-gray-800 border-solid rounded-lg"
     pt:title:class="flex justify-center mt-8"
     >
        <template #title>
            <span class="text-2xl text-gray-200">Login</span>
        </template>
        <template #content>
            <div class="m-12 space-y-8">
                <FloatLabel variant="on">
                    <InputText v-mode="username" id="username" type="text" class="border border-solid rounded-lg bg-gray-50" size="large" fluid></InputText>
                    <label for="username">Username</label>
                </FloatLabel>
                <FloatLabel variant="on">
                    <Password v-model="password" id="password" class="border border-solid rounded-lg bg-gray-50" size="large" fluid></Password>
                    <label for="password">Password</label>
                </FloatLabel>
                <div class="flex justify-center">   
                    <a href="" class="text-gray-500 hover:text-emerald-500 cursor-pointer">Click here to sign up</a>
                </div>
            </div>
        </template>
        <template #footer>
            <div class="flex gap-4 mt-1">
                <Button label="Submit" class="w-full border border-gray-200" />
            </div>
        </template>
    </Card>
</template>

<script setup>
import Card from 'primevue/card';
import InputText from 'primevue/inputtext';
import FloatLabel from 'primevue/floatlabel';
import Button from 'primevue/button';
import Password from 'primevue/password';
import { ref } from 'vue';

const username = ref(null);
const password = ref(null);


</script>