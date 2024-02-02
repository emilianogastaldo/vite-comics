<script>
export default {
    name: 'FooterMenu',
    props: {
        menu: Object
    }
}
</script>

<template>
    <h4>{{ menu.title }}</h4>
    <ul>
        <li v-for="(link, i) in menu.links" :key="i">
            <a :href="link.href">{{ link.text }}</a>
        </li>
    </ul>
</template>

<style lang="scss" scoped>
h4 {
    text-transform: uppercase;
    font-size: larger;
}

ul {
    margin: 1rem 0;

    li a {
        font-family: 'Open Sans', sans-serif;
        color: #818181;
        text-transform: capitalize;
        font-size: small;
        line-height: 1.3rem;

        &:hover {
            color: white;
        }
    }

}
</style>