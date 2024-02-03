<script>
import BlueSectionLink from './blue-section-components/BlueSectionLink.vue';
export default {
    name: 'AppBlueSection',
    props: {
        links: Array
    },
    components: {
        BlueSectionLink
    }
}
</script>

<template>
    <section>
        <ul class="wrapper flex">
            <li v-for="link in links" :key="link.text">
                <BlueSectionLink :icon="link" />
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
</style>