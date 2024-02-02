
<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import AppBlueSection from './components/AppBlueSection.vue';
import { footerMenus } from './assets/data/index.js';

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
    })
}
</script>
 
<template>
    <AppHeader />
    <AppMain />
    <AppBlueSection />
    <AppFooter :menus="footerMenus" />
</template>

<style lang="scss">
@use 'assets/scss/style.scss';
</style>
