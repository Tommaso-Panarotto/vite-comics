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
            <button>
                LOAD MORE
            </button>
        </div>
    </main>
</template>

<style lang="scss" scoped>
main {
    background-color: #1C1C1C;
    text-align: center;

    button {
        padding: 10px 35px;
        margin: 35px 0 20px 0;
        border: 0;
        cursor: pointer;
        background-color: #0282F9;
        color: white;
    }

    #content {
        color: white;
        text-transform: uppercase;
        font-weight: bold;

        ul {
            display: flex;
            flex-wrap: wrap;
            gap: 20px 20px;
        }
    }
}
</style>