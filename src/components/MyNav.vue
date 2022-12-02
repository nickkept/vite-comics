<template>
    <header>
        <div class="container py-3 d-flex justify-content-between align-items-baseline">
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
// @use "./partials/variables" as *;
    ul{
        list-style: none;
        a{
        text-decoration: none;
        margin-left: 1rem;
        font-weight: bold;
        color: #303030;
    }
    }
</style>