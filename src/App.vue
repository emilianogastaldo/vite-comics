
<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import AppBlueSection from './components/AppBlueSection.vue';

export default {
    name: 'App',
    components: {
        AppHeader,
        AppMain,
        AppFooter,
        AppBlueSection,
    }
}
</script>
 
<template>
    <AppHeader />
    <AppMain />
    <AppBlueSection />
    <AppFooter />
</template>

<style lang="scss">
@use 'assets/scss/style.scss';
</style>
