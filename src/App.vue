
<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
export default {
    name: 'App',
    components: {
        AppHeader,
        AppMain,
    }
}
</script>
 
<template>
    <AppHeader />
    <AppMain />
    <h1>prova</h1>
</template>

<style>
h1 {
    color: red;
}
</style>
