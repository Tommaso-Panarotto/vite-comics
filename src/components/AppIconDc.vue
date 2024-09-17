<script>
export default {
    data() {
        return {
            icons: [
                { name: "digital comics", imageUrl: "buy-comics-digital-comics.png" },
                { name: "dc merchandise", imageUrl: "buy-comics-merchandise.png" },
                { name: "subscription", imageUrl: "buy-comics-subscriptions.png" },
                { name: "comic shop locator", imageUrl: "buy-comics-shop-locator.png" },
                { name: "dc power visa", imageUrl: "buy-dc-power-visa.svg" }
            ]
        }
    },
    methods: {
        getImageUrl(imageUrl) {
            return new URL(`../assets/img/${imageUrl}`, import.meta.url).href;
        }
    }
}
</script>

<template>
    <div class="icons-link">
        <div class="container">
            <ul>
                <li v-for="icon in icons"><img :src="getImageUrl(icon.imageUrl)" :alt="icon.name">
                    <p>{{ icon.name.toUpperCase() }}</p>
                </li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.icons-link {
    height: 150px;
    background-color: #0282F9;
    position: relative;
    z-index: 1;

    ul {
        display: flex;
        justify-content: space-around;
        height: 100%;

        li {
            width: calc((100% / 5) - 35px);
            display: flex;
            align-items: center;
            gap: 20px;
            color: white;
            cursor: pointer;

            img {
                max-height: 60px;
            }
        }
    }
}
</style>