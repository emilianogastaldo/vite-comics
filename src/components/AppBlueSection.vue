<script>
export default {
    name: 'AppBlueSection',
    data: () => ({
        buyList: [
            {
                text: 'digital comics',
                imgurl: 'buy-comics-digital-comics.png'
            },
            {
                text: 'dc merchandise',
                imgurl: 'buy-comics-merchandise.png'
            },
            {
                text: 'subscription',
                imgurl: 'buy-comics-subscriptions.png'
            },
            {
                text: 'comic shop locator',
                imgurl: 'buy-comics-shop-locator.png'
            },
            {
                text: 'dc power visa',
                imgurl: 'buy-dc-power-visa.svg'
            },
        ]
    })
}
</script>

<template>
    <section>
        <ul class="wrapper">

            LISTA
        </ul>
    </section>
</template>
<style lang="scss" scoped>
section {
    background-color: #0282F9;
    color: white;
    padding: 10px 0;
}
</style>