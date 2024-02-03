<script>
export default {
    name: 'AppHeader',
    data: () => ({
        links: [
            { text: 'Characters', url: '#', current: false, },
            { text: 'Comics', url: '#', current: true, },
            { text: 'Movies', url: '#', current: false, },
            { text: 'TV', url: '#', current: false, },
            { text: 'Games', url: '#', current: false, },
            { text: 'Collectibles', url: '#', current: false, },
            { text: 'Videos', url: '#', current: false, },
            { text: 'Fans', url: '#', current: false, },
            { text: 'News', url: '#', current: false, },
            { text: 'Shop', url: '#', current: false, },
        ]
    })
}
</script>

<template >
    <header>
        <div class="wrapper flex">
            <figure>
                <a href="#"><img src="../assets/img/logos/dc-logo.png" alt=""></a>
            </figure>
            <nav>
                <ul class="flex">
                    <li v-for="link in links"><a :href="link.url" :class="{ active: link.current }">{{ link.text }}</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style lang="scss" scoped>
header {
    background-color: #FFFFFF;
    height: 100px;
    line-height: 100px;

    ul {
        gap: 2rem;

        li a {
            text-transform: uppercase;
            color: #484848;
            padding: 37px 0;
            font-size: 0.8rem;
            font-weight: 700;

            &:hover,
            &.active {
                color: #0282F9;
                border-bottom: 5px solid #0282F9;
            }
        }
    }
}

figure {
    height: 70px;
}
</style>
