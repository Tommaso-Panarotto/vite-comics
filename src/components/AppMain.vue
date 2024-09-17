<script>
import ComicsList from "./ComicsList.vue";
import AppMainJumbotron from "./AppMainJumbotron.vue";

export default {
    data() {
        return {

        }
    },
    components: {
        ComicsList,
        AppMainJumbotron
    }
}
</script>

<template>
    <main>
        <AppMainJumbotron />
        <div class="container">
            <section id="content">
                <ComicsList />
            </section>
        </div>
    </main>
</template>

<style lang="scss" scoped>
main {
    background-color: #1C1C1C;
    height: 140px;

    #content {
        line-height: 120px;
        color: white;
        font-size: 2rem;
        font-weight: bold;
    }
}
</style>