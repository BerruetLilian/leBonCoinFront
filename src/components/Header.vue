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
                            <font-awesome-icon :icon="['fa', 'plus-square']" />
                            <span>Déposer une annonce</span>
                        </RouterLink>
                    </div>
                    <div class="search-input">
                        <input type="text" name="search" placeholder="Rechercher sur leboncoin" />
                        <button>
                            <font-awesome-icon :icon="['fas', 'search']" />
                        </button>
                    </div>
                </div>
                <div class="right">
                    <RouterLink to="/login">
                        <font-awesome-icon :icon="['fas', 'user']" />
                        <p>Se connecter</p>
                    </RouterLink>
                </div>
            </div>
            <div class="bottom">
                <span>Immobilier</span>
                <font-awesome-icon :icon="['fas', 'circle']" />
                <span>Immobilier</span>
                <font-awesome-icon :icon="['fas', 'circle']" />
                <span>Véhicules</span>
                <font-awesome-icon :icon="['fas', 'circle']" />
                <span>Location de vacances</span>
                <font-awesome-icon :icon="['fas', 'circle']" />
                <span>Emploi</span>
                <font-awesome-icon :icon="['fas', 'circle']" />
                <span>Mode</span>
                <font-awesome-icon :icon="['fas', 'circle']" />
                <span>Maison & Jardin</span>
                <font-awesome-icon :icon="['fas', 'circle']" />
                <span>Famille</span>
                <font-awesome-icon :icon="['fas', 'circle']" />
                <span>Electronique</span>
                <font-awesome-icon :icon="['fas', 'circle']" />
                <span>Loisirs</span>
                <font-awesome-icon :icon="['fas', 'circle']" />
                <span>Autres</span>
            </div>
        </div>
    </header>
</template>

<style scoped>
.bottom svg {
    color: var(--black);
    font-size: 2px;
}

.bottom {
    display: flex;
    justify-content: space-between;
    align-items: center;
    font-size: 14px;
}

header {
    border-bottom: 1px solid var(--grey);
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    background-color: #fff;
    z-index: 5;
    height: var(--header-height);
}

.right {
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
}

.right p {
    font-size: 12px;
}

.search-input svg {
    background-color: var(--orange);
    padding: 8px;
    border-radius: 7px;
}

.search-input button {
    display: flex;
    align-items: center;
    border: none;
    background-color: #fff0;
    padding: 0;
}

.search-input input {
    border: none;
    flex: 1;
    outline: none;
    background-color: inherit;
}

.search-input {
    display: flex;
    padding: 7px;
    border-radius: 10px;
    width: 300px;
    background-color: var(--grey-light);
}

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