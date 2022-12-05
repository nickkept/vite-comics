<template>
    <div class="footer-section">
        <div class="container">
            <div class="row">
                <div class="col-4 d-flex">
                    <div class="col py-4 d-block">
                        <ul>
                            <li>
                                <h6>DC COMICS</h6>
                            </li>
                            <li v-for="element in dcComicsList">
                                <a :href="element.url">{{ element.text }}</a>
                            </li>
                        </ul>
                        <ul>
                            <li>
                                <h6>SHOP</h6>
                            </li>
                            <li v-for="element in shopList">
                                <a :href="element.url">{{ element.text }}</a>
                            </li>
                        </ul>
                    </div>
                    <div class="col py-4">
                        <ul>
                            <li>
                                <h6>DC</h6>
                            </li>
                            <li v-for="element in dcList">
                                <a :href="element.url">{{ element.text }}</a>
                            </li>
                        </ul>
                    </div>
                    <div class="col py-4">
                        <ul>
                            <li>
                                <h6>SITES</h6>
                            </li>
                            <li v-for="element in sitesList">
                                <a :href="element.url">{{ element.text }}</a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
            <!-- <div class="row d-flex">
                <div class="col">
                    <ul>
                        <li>
                            <h5>DC COMICS</h5>
                        </li>
                        <li v-for="element in dcComicsList">
                            <a :href="element.url">{{ element.text }}</a>
                        </li>
                    </ul>
                    <ul>
                        <li>
                            <h5>SHOP</h5>
                        </li>
                        <li v-for="element in shopList">
                            <a :href="element.url">{{ element.text }}</a>
                        </li>
                    </ul>
                </div>
                <ul>
                    <li>
                        <h5>DC</h5>
                    </li>
                    <li v-for="element in dcList">
                        <a :href="element.url">{{ element.text }}</a>
                    </li>
                </ul>
                <ul>
                    <li>
                        <h5>SITES</h5>
                    </li>
                    <li v-for="element in sitesList">
                        <a :href="element.url">{{ element.text }}</a>
                    </li>
                </ul>
            </div> -->
        </div>
    </div>
</template>
<script>
export default {
    data() {
        return {
            dcComicsList: [
                {
                    text: 'Characters',
                    url: '#'
                },
                {
                    text: 'Comics',
                    url: '#'
                },
                {
                    text: 'Movies',
                    url: '#'
                },
                {
                    text: 'TV',
                    url: '#'
                },
                {
                    text: 'Games',
                    url: '#'
                },
                {
                    text: 'Videos',
                    url: '#'
                },
                {
                    text: 'News',
                    url: '#'
                },
            ],
            shopList: [
                {
                    text: 'Shop DC',
                    url: '#'
                },
                {
                    text: 'Shop DC Collections',
                    url: '#'
                },
            ],
            dcList: [
                {
                    text: 'Terms Of Use',
                    url: '#'
                },
                {
                    text: 'Privacy Policy (New)',
                    url: '#'
                },
                {
                    text: 'Ad Choices',
                    url: '#'
                },
                {
                    text: 'Advertising',
                    url: '#'
                },
                {
                    text: 'Jobs',
                    url: '#'
                },
                {
                    text: 'Subscriptions',
                    url: '#'
                },
                {
                    text: 'Talent Workspace',
                    url: '#'
                },
                {
                    text: 'CPSC Certnificates',
                    url: '#'
                },
                {
                    text: 'Ratings',
                    url: '#'
                },
                {
                    text: 'Shop Help',
                    url: '#'
                },
                {
                    text: 'Contact US',
                    url: '#'
                },
            ],
            sitesList: [
                {
                    text: 'DC',
                    url: '#'
                },
                {
                    text: 'MAD Magazine',
                    url: '#'
                },
                {
                    text: 'DC Kids',
                    url: '#'
                },
                {
                    text: 'DC Universe',
                    url: '#'
                },
                {
                    text: 'DC Power Visa',
                    url: '#'
                },
            ]
        }
    }
};

</script>
<style scoped lang="scss">
// @use "./partials/variables" as *;
.footer-section {
    background-image: url('/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    .container {
        // padding: 1.5rem 0;
        background-image: url('/dc-logo-bg.png');
        background-repeat: no-repeat;
        background-position: right;
            ul {
                list-style: none;
                // margin-right: 1rem;
                h6 {
                    color: white;
                    // margin-bottom: 1.2rem;
                }
                a {
                    color: #797979;
                    text-decoration: none;
                    // margin-bottom: 0.5rem;
                    display: block;
                    font-size: .7rem;
                    margin-left: 0;
                }
            }
    }
}
</style>