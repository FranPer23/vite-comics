<script>
    export default {
        name: "AppHeader",
        data(){
            return {
                links: [
                {
                    text: "Characters",
                    url: "#",
                    current: false
                },
                {
                    text: "Comics",
                    url: "#",
                    current: true
                },
                {
                    text: "Movies",
                    url: "#",
                    current: false
                },
                {
                    text: "Tv",
                    url: "#",
                    current: false
                },
                {
                    text: "Games",
                    url: "#",
                    current: false
                },
                {
                    text: "Collectibles",
                    url: "#",
                    current: false
                },
                {
                    text: "Videos",
                    url: "#",
                    current: false
                },
                {
                    text: "Fans",
                    url: "#",
                    current: false
                },
                {
                    text: "News",
                    url: "#",
                    current: false
                },
                {
                    text: "Shop",
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
    </header>
</template>

<style scope lang="scss">

</style>

