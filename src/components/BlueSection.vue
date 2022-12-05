<template>
    <main class="blue-section py-5">
        <div class="container">
            <div class="d-flex my-icons ">
                <div class="d-flex align-items-center text-white px-3" v-for="item in items">
                    <img class="blue-images" :src="item.image" alt="">
                    <a class="text-white px-2" href="/">{{item.name}}</a>
                </div>
            </div>
        </div>
    </main>
</template>
<script>
export default {
    data() {
        return {
            items: [
        {
            image: "/buy-comics-digital-comics.png",
            name: "DIGITAL COMICS",
        },
        {
            image: "/buy-comics-merchandise.png",
            name: "DC MERCHANDISE",
        },
        {
            image: "/buy-comics-subscriptions.png",
            name: "SUBSCRIPTION",
        },
        {
            image: "/buy-comics-shop-locator.png",
            name: "COMIC SHOP LOCATOR",
        },
        {
            image: "/buy-dc-power-visa.svg",
            name: "DC POWER VISA",
        },
    ],
            // images:[
            // "/buy-comics-digital-comics.png",
            // "/buy-comics-merchandise.png",
            // "/buy-comics-subscriptions.png",
            // "/buy-comics-shop-locator.png",
            // "/buy-dc-power-visa.svg"
            // ]
        };
},
methods: {},
};
</script>
<style scoped lang="scss">
// @use "./partials/variables" as *;
    .blue-section{
        background-color: #0082F9;
        .blue-images{
            height: 50px;
            display: block;
            // width: 100%;
            aspect-ratio: 1/1;
        }
        a{
            text-decoration: none;
        }
        .my-icons{
            margin-left: 4rem;
        }
    }
</style>