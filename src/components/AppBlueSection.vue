<script>
export default {
    name: 'AppBlueSection',
    props: {
        links: Object
    },
    methods: {
        imgUrl(subString) {
            return new URL(`../assets/img/section_blue_icons/${subString}`, import.meta.url).href
        }
    }
}
</script>

<template>
    <section>
        <ul class="wrapper flex">
            <li v-for="link in links" :key="link.text">
                <a href="#">
                    <img :src="imgUrl(link.img)" alt="img">
                    {{ link.text }}
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

ul {
    padding: 0 1rem;

    li {
        flex-basis: calc(100%/5);
    }
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
        display: block;
        max-width: 50px;
        max-height: 50px;
    }
}
</style>