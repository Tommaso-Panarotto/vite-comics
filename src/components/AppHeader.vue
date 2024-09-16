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
                <img src="../assets/dc-logo.png" alt="DC Main Logo">
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
    width: 100%;
    height: 100px;

    .container {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    #logo {
        width: 80px;
        height: 80px;
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
            text-transform: uppercase;
            font-weight: bold;
            border-bottom: 7px solid white;

            &:active,
            &:hover {
                border-bottom: 7px solid #0282F9;
            }

            a {
                color: #666161;
            }

            &:active a,
            &:hover a {
                color: #0282F9;
            }
        }
    }
}
</style>