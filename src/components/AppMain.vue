<script>
export default {
    data() {
        return {

        }
    }
}
</script>

<template>
    <main>
        <div class="container">
            <section id="content">
                <p>--Content goes here--</p>
            </section>
        </div>
    </main>
</template>

<style lang="scss" scoped>
main {
    background-color: #1C1C1C;
    height: 140px;
    position: relative;
    z-index: 1;

    #content {
        line-height: 120px;
        color: white;
        font-size: 2rem;
        font-weight: bold;
    }
}
</style>