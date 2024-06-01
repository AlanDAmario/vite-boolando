<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
export default {
    name: 'MyApp',
    components: {
        AppHeader,
        AppMain,
        AppFooter,
    }
}

</script>

<template>
    <body>
        <AppHeader />
        <AppMain />
        <AppFooter />
    </body>
</template>

<style></style>

