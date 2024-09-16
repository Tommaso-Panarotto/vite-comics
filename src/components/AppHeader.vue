<script>
export default {
    data() {
        return {
            headerLinks: [
                "Characters",
                "Comics",
                "Movies",
                "Tv",
                "Games",
                "Collectible",
                "Videos",
                "Fans",
                "News",
                "Shop"
            ]

        }
    }
}
</script>

<template>
    <header>
        <div class="container">
            <!--LOGO-->
            <section id="logo">
                LOGO
            </section>

            <!--LINKS-->
            <nav id="navbar-links">
                <ul>
                    <li v-for="link in headerLinks"><a href="#">{{ link }}</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style lang="scss" scoped>
header {
    background-color: aqua;
    width: 100%;
    height: 100px;

    .container {
        height: 100%;
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    #logo {
        background-color: yellow;
        width: 100px;
        text-align: center;
    }

    nav {
        height: 100%;
    }

    ul {
        height: 100%;
        display: flex;

        li {
            line-height: 100px;
            height: 100%;
            padding: 0 10px;

            border-bottom: 10px solid white;
        }
    }
}
</style>