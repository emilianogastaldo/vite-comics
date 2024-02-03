
<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import AppBlueSection from './components/AppBlueSection.vue';
import { headerLinks, blueSectionLinks, footerMenus, footerIcons } from './assets/data/index.js';

export default {
    name: 'App',
    components: {
        AppHeader,
        AppMain,
        AppFooter,
        AppBlueSection
    },
    data: () => ({
        footerMenus,
        footerIcons,
        blueSectionLinks,
        headerLinks,
    })
}
</script>
 
<template>
    <AppHeader :links="headerLinks" />
    <AppMain />
    <AppBlueSection :links="blueSectionLinks" />
    <AppFooter :menus="footerMenus" :icons="footerIcons" />
</template>

<style lang="scss">
@use 'assets/scss/style.scss';
</style>
