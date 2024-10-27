<template>
    <div class="login-card-container">
        <div class="login-card">
            <LoginCard/>
        </div>
    </div>
</template>

<script setup>
import LoginCard from '../Components/LoginCard.vue'
</script>

<style lang="css" scoped>
    .login-card-container {
        display: flex;
        min-height: 100vh;
        align-items: center;
        justify-content: center;
    }

    .login-card {
        max-width: 35%;
    }
</style>