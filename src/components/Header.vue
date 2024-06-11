<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
    <header>
        <ul>
            <li>
                <RouterLink to="/">Home</RouterLink>
            </li>
            <li>
                <RouterLink to="/profile">My profile</RouterLink>
            </li>
            <li>
                <RouterLink to="/contact">Contact</RouterLink>
            </li>
        </ul>
    </header>
</template>

<style lang="scss">
header {
    z-index: 1;
    position: fixed;
    top: 0;
    width: 100%;
    height: 10%;
    display: flex;
    justify-content: end;
    text-align: center;
    align-items: center;
    background-color: #1F213B;
    color: white;

    ul {
        display: flex;
        list-style: none;
        width: 50%;
        justify-content: space-around;
        background-color: #1F213B;

        li {
            position: relative;
            transition: all 0.1s linear;
            background-color: #1F213B;

            :visited {
                color: white;
                background-color: #1F213B;
            }

            &:after {
                content: "";
                position: absolute;
                bottom: -3px;
                left: 0;
                background-color: #b94e56;
                height: 3px;
                width: 0;
                transition: width 0.3s ease;
                border-radius: 5px;
            }

            &:hover::after {
                width: 100%;
            }
        }
    }
}
</style>
