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

    #content {
        color: white;
        text-transform: uppercase;
        font-weight: bold;

        ul {
            display: flex;
            gap: 10px;

            li {
                width: calc((100% / 6) - 10px);
            }
        }
    }
}
</style>