<template>
    <header>
        <div class="container d-flex justify-content-between align-items-baseline">
            <div>
                <img src="/dc-logo.png" alt="">
            </div>
            <div>
                <ul class="d-flex">
                    <li v-for="(link) in links">
                        <a href="">{{link}}</a>
                    </li>
                </ul>
            </div>
        </div>
    </header>
</template>
<script>
export default {
    data() {
        return {
            links: [
            "CHARACTERS",
            "COMICS",
            "MOVIES",
            "TV",
            "GAMES",
            "COLLECTIBLES",
            "VIDEOS",
            "FANS",
            "NEWS",
            "SHOP",
        ],
        };
},
methods: {},
};
</script>
<style lang="scss">
    ul{
        list-style: none;
        a{
        text-decoration: none;
    }
    }
</style>