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
        <ul class="wrapper flex space-around">
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