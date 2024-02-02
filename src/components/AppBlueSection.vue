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
    })
}
</script>

<template>
    <section>
        <<<<<<< HEAD <ul class="wrapper">

            LISTA
            =======
            <ul class="wrapper flex space-around">
                <li v-for="item in buyList">
                    <a href="#">
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                        {{ item.text }}
                    </a>
                </li>
                >>>>>>> AppBlueSection
            </ul>
    </section>
</template>
<style lang="scss" scoped>
section {
    background-color: #0282F9;
    <<<<<<< HEAD color: white;
    padding: 10px 0;
    =======padding: 3rem 0;

}

a {
    height: 70px;
    font-family: "Open Sans", sans-serif;
    color: white;
    text-transform: uppercase;
    font-size: 14px;
    display: flex;
    align-items: center;
    gap: 1rem;
    >>>>>>>AppBlueSection
}
</style>