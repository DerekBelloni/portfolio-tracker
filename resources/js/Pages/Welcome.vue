<template>
    <div class="welcome-card-container">
        <div class="welcome-card">
            <component :is="!registrationActive ? LoginCard : RegistrationCard" @toggleActive="toggleActive()"/>
        </div>
    </div>
</template>

<script setup>
import LoginCard from '../Components/LoginCard.vue'
import RegistrationCard from '@/Components/RegistrationCard.vue';
import { reactive, ref, onBeforeMount, shallowRef } from 'vue';

const registrationActive = ref(false);

function toggleActive(toggleTo) {
    registrationActive.value = !registrationActive.value;
}

</script>

<style lang="css" scoped>
    .welcome-card-container {
        display: flex;
        min-height: 100vh;
        align-items: center;
        justify-content: center;
    }

    .welcome-card {
        max-width: 35%;
    }
</style>