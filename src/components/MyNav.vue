<template>
    <header>
        <div class="container ">
            <div class="py-3 d-flex justify-content-between align-items-baseline">
                <div>
                    <img src="/dc-logo.png" alt="">
                </div>
                <div>
                    <ul class="d-flex nav-links">
                        <li v-for="(link) in links">
                            <a href="">{{link}}</a>
                        </li>
                    </ul>
                </div>
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
<style scoped lang="scss">
// @use "../styles/partials/variables" as *;
.nav-links{
    margin-right: 5rem;
    list-style: none;
    a{
        text-decoration: none;
        margin-left: 1rem;
        font-weight: bold;
        font-size: .8rem;
        color: #797979;
    }
    
}
</style>