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
            <div class="current-series"><span>current series</span></div>
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

    .container {
        position: relative;

        .current-series {
            width: 300px;
            height: 50px;
            line-height: 50px;
            background-color: #0282F9;
            color: white;
            text-transform: uppercase;
            font-weight: bold;
            font-size: 25px;
            position: absolute;
            left: 0;
            top: -25px;
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

        button {
            padding: 10px 35px;
            margin: 35px 0 20px 0;
            border: 0;
            cursor: pointer;
            background-color: #0282F9;
            color: white;
        }
    }
}
</style>