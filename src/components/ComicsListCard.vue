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
        <img :src="comicImageUrl" :alt="comicName">
        {{ comicName }}
    </li>
</template>

<style lang="scss" scoped></style>