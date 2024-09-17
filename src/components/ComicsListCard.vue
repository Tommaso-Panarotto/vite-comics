<script>
export default {
    data() {
        return {

        }
    },
    props: {
        comicImageUrl: {
            type: String,
            required: true
        },
        comicName: {
            type: String,
            required: true
        }
    }
}
</script>

<template>
    <li>
        <div class="comic-image">
            <img :src="comicImageUrl" :alt="comicName">
        </div>
        {{ comicName }}
    </li>
</template>

<style lang="scss" scoped>
li {
    width: calc((100% / 6) - 20px);
    height: 400px;
    border: 1px solid #1C1C1C;

    &:hover {
        border: 1px solid white;
    }

    .comic-image {
        height: 350px;
        display: flex;
        align-items: center;
        justify-content: center;
    }
}
</style>