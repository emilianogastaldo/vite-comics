
<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';

export default {
    name: 'App',
    components: {
        AppHeader,
        AppMain,
        AppFooter,
    }
}
</script>
 
<template>
    <AppHeader />
    <AppMain />
    <AppFooter />
</template>

<style>
* {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}

body {
    background-color: black;
    font-family: 'Roboto Condensed', sans-serif;
}

a {
    text-decoration: none;
}

ul {
    list-style-type: none;
}
</style>
