<script>
export default {
    name: 'FooterIcon',
    props: {
        icon: Object
    },

    computed: {
        iconPath() {
            return new URL(`../../assets/img/footer_images/${this.icon.img}`, import.meta.url).href
        }
    }

}
</script>

<template>
    <!-- <a href="#"><img :src="this.img" alt="#"></a> -->
    <a :href="icon.href"><img :src="this.iconPath" :alt="icon.name"></a>
</template>

<style lang="scss" scoped>
img:hover {
    filter: brightness(200%);
}
</style>