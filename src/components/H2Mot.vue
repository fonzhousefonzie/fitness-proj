<template>
    <div class="mot">
        <h2>{{h2}}</h2>
        <img src="../assets/img/sep.svg" class="separator mt-4 mb-2">
        <div class="credit d-flex justify-content-center align-items-center gap-3">
            <img :src="img" alt="">
            <h6 class="text-light">{{whiteText}}</h6>
            <h6>{{text}}</h6>
        </div>
        <div v-html="element" class="element"></div>
    </div>
</template>

<script>
export default {
    props:{
        h2: String,
        img: String,
        whiteText: String,
        text: String,
        element: Element
    }
}
</script>

<style lang="scss" scoped>
.mot {
    padding: 2rem 0 3rem;
    margin: auto;
    width: 75%;

    h2 {
        color: white;
        font-weight: bold;
    }

    .credit {
        width: 100%;

        img {
            max-width: 60px;
            border-radius: 50%;
        }

        h6 {
            color: var(--light-grey);
            margin-bottom: 0;
        }

        h6.text-light{
            font-weight: bold;
        }
    }

    .element{
        margin-top: 1rem;
    }

}
</style>