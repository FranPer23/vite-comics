<script>
    export default {
        name: "AppHeader",
        data(){
            return {
                links: [
                {
                    text: "CHARACTERS",
                    url: "#",
                    current: false
                },
                {
                    text: "COMICS",
                    url: "#",
                    current: true
                },
                {
                    text: "MOVIES",
                    url: "#",
                    current: false
                },
                {
                    text: "TV",
                    url: "#",
                    current: false
                },
                {
                    text: "GAMES",
                    url: "#",
                    current: false
                },
                {
                    text: "COLLECTIBLES",
                    url: "#",
                    current: false
                },
                {
                    text: "VIDEOS",
                    url: "#",
                    current: false
                },
                {
                    text: "FANS",
                    url: "#",
                    current: false
                },
                {
                    text: "NEWS",
                    url: "#",
                    current: false
                },
                {
                    text: "SHOP",
                    url: "#",
                    current: false
                },
            ]
            }

        }
    }
</script>

<template>
    <header>
        <div class="top">
            
        </div>
        <nav class="bottom flex">
            <a href="">
                <img class="logo" src="../assets/img/dc-logo.png" alt="">
            </a>
            <ul class="header-nav flex">
                <li v-for="link in links" :class="link.current ? 'active' : ''">
                    <a :href="link.url">{{ link.text }}</a>
                </li>
            </ul>
        </nav>
        <div class="bottom-nav">
            
        </div>
    </header>
</template>

<style scope lang="scss">

.header-nav li.active a {
        color: #0282f9;
        position: relative;
    }

.header-nav li.active a::after {
        content: "";
        position: absolute;
        left: 0;
        bottom: -30px;
        width: 100%;
        height: 2px;
        background-color: #0282f9;
    }

</style>

