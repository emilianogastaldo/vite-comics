<script>
export default {
    name: 'BlueSectionLink',
    props: {
        icon: Object,
    },
    computed: {
        iconImg() {
            return new URL(`../../assets/img/section_blue_icons/${this.icon.img}`, import.meta.url).href
        }
    }
}
</script>

<template>
    <a :href="icon.url">
        <img :src="iconImg" alt="icon.text">
        {{ icon.text }}
    </a>
</template>

<style lang="scss" scoped>
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