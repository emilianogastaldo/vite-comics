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
        <div class="container flex">
            <figure>
                <img src="../assets/img/dc-logo.png" alt="">
            </figure>
            <nav>
                <ul class="flex">
                    <li v-for="link in links"><a :href="link.url">{{ link.text }}</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style scoped>
header {
    background-color: #FFFFFF;
    margin-top: 1rem;
    padding: 1rem 0;
    height: 100px;

}

figure {
    width: 70px;
}



.container {
    max-width: 1200px;
    margin: 0 auto;
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
    padding: 1rem 0;
    color: #484848;
    flex-shrink: 1;
}

ul li a:hover {
    color: #0282F9;
    border-bottom: 4px solid #0282F9;
}
</style>
