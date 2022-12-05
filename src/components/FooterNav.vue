<template>
    <div class="footer-nav">
        <div class="container">
            <div class="d-flex justify-content-between align-items-center py-4">
                <button>SIGN-UP NOW</button>
                <div class="d-flex align-items-center">
                    <a href="#">FOLLOW US</a>
                    <div class="d-flex align-items-center">
                        <a v-for="icon in iconsList" href="#">
                            <img :src="`/footer-${icon}.png`">
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>



<script>
export default {
    data() {
        return {
            iconsList: [
                'facebook',
                'twitter',
                'youtube',
                'pinterest',
                'periscope',
            ]
        }
    }
}
</script>



<style scoped lang="scss">
.footer-nav{
    background-color: #303030;
        button {
            background-color: transparent;
            border: 3px solid #0382f9;
            color: white;
            font-size: .8rem;
            padding: 1rem;
        }
        div {
            a {
                text-decoration: none;
                font-weight: bold;
                font-size: 1.2rem;
                color: #0382f9;
            }
            div {
                a {
                    img {
                        height: 100%;
                        margin: 0 0.4rem;
                        aspect-ratio: 1/1;
                    }
                }
            }
        }
}
</style>