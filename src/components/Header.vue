<script setup>
import { RouterLink } from 'vue-router';
import logo from "../assets/img/logo.svg";
</script>

<template>
    <header>
        <div class="container">
            <div class="top">
                <RouterLink to="/">
                    <img :src="logo" alt="logo-leboncoin">
                </RouterLink>
                <div class="middle">
                    <div class="publish-btn">
                        <RouterLink to="/publish">
                            <font-awesome-icon :icon="['far', 'square-plus']" />
                            <span>Déposer une annonce</span>
                        </RouterLink>
                    </div>
                    <div class="search-input">

                    </div>
                </div>
                <div class="right">

                </div>
            </div>
        </div>
    </header>
</template>

<style scoped>
.container {
    padding: 10px 0 20px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}

.top {
    display: flex;
    justify-content: space-between;
}

img {
    width: 140px;
}

.middle {
    display: flex;
    align-items: center;
    gap: 20px;
}

.publish-btn {
    background-color: var(--orange);
    color: white;
    padding: 10px;
    border: none;
    border-radius: 10px;
    font-weight: 700;
}
</style>