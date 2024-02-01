<script>
export default {
    name: 'AppHeader',
    data: () => ({
        links: [
            {
                text: 'Characters',
                url: '#',
                current: false,
            },
            {
                text: 'Comics',
                url: '#',
                current: true,
            },
            {
                text: 'Movies',
                url: '#',
                current: false,
            },
            {
                text: 'TV',
                url: '#',
                current: false,
            },
            {
                text: 'Games',
                url: '#',
                current: false,
            },
            {
                text: 'Collectibles',
                url: '#',
                current: false,
            },
            {
                text: 'Videos',
                url: '#',
                current: false,
            },
            {
                text: 'Fans',
                url: '#',
                current: false,
            },
            {
                text: 'News',
                url: '#',
                current: false,
            },
            {
                text: 'Shop',
                url: '#',
                current: false,
            },
        ]
    })
}
</script>

<template >
    <header>
        <div class="wrapper flex">
            <figure>
                <a href="#"><img src="../assets/img/dc-logo.png" alt=""></a>
            </figure>
            <nav>
                <ul class="flex">
                    <li v-for="link in links"><a :href="link.url" :class="{ active: link.current }">{{ link.text }}</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style scoped>
header {
    background-color: #FFFFFF;
    margin-top: 1rem;
    height: 100px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-basis: 100%;
}

figure {
    width: 70px;
}



.wrapper {
    width: 1200px;
}

.flex {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

ul {
    gap: 2rem;
}

ul li a {
    text-transform: uppercase;
    color: #484848;
    padding: 36px 0;
}

ul li a:hover,
ul li a.active {
    color: #0282F9;
    border-bottom: 5px solid #0282F9;
}
</style>
