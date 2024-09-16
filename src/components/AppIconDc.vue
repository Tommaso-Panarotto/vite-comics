<script>
export default {
    data() {
        return {
            icons: [
                { name: "digital comics", image: "../assets/buy-comics-digital-comics.png" },
                { name: "dc merchandise", image: "../assets/buy-comics-merchandise.png" },
                { name: "subscription", image: "../assets/buy-comics-subscription.png" },
                { name: "comic shop locator", image: "../assets/buy-comics-shop-locator.png" },
                { name: "dc power visa", image: "../assets/buy-dc-power-visa.svg" }
            ]
        }
    }
}
</script>

<template>
    <div class="icons-link">
        <div class="container">
            <ul>
                <li v-for="icon in icons"><img src="../assets/buy-comics-merchandise.png" alt="icon.name">
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
            display: flex;
            align-items: center;
            gap: 20px;
            color: white;

            img {
                width: 60px;
            }
        }
    }
}
</style>