<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";
import AppIconDc from "./components/AppIconDc.vue";

export default {
    data() {
        return {

        }
    },
    components: {
        AppHeader,
        AppMain,
        AppFooter,
        AppIconDc
    }
}
</script>

<template>
    <AppHeader />
    <AppMain />
    <AppIconDc />
    <AppFooter />
</template>

<style lang="scss">
@use "./styles/general.scss" as *;
</style>
