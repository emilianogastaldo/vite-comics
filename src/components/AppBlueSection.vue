<script>
export default {
    name: 'AppBlueSection',
    data: () => ({
        buyList: [
            {
                text: 'digital comics',
                img: 'buy-comics-digital-comics.png',
                url: '#'
            },
            {
                text: 'dc merchandise',
                img: 'buy-comics-merchandise.png',
                url: '#'
            },
            {
                text: 'subscription',
                img: 'buy-comics-subscriptions.png',
                url: '#'
            },
            {
                text: 'comic shop locator',
                img: 'buy-comics-shop-locator.png',
                url: '#'
            },
            {
                text: 'dc power visa',
                img: 'buy-dc-power-visa.svg',
                url: '#'
            },
        ]
    }),
    methods: {
        imgUrl(subString) {
            return new URL(`../assets/img/${subString}`, import.meta.url).href
        }
    }
}
</script>

<template>
    <section>
        <ul class="wrapper flex space-around">
            <li v-for="item in buyList">
                <a href="#">
                    <img :src="imgUrl(item.img)" alt="img">
                    {{ item.text }}
                </a>
            </li>
        </ul>
    </section>
</template>
<style lang="scss" scoped>
section {
    background-color: #0282F9;
    color: white;
    padding: 3rem 0;

}

a {
    font-family: "Open Sans", sans-serif;
    color: white;
    text-transform: uppercase;
    font-size: 14px;
    display: flex;
    align-items: center;
    gap: 1rem;

    img {
        width: 50px;
    }
}
</style>