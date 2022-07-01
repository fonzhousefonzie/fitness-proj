<template>
    <div class="mot col-65">
        <h2>{{h2}}</h2>
        <img src="../assets/img/sep.svg" class="separator mt-4 mb-2">
        <div class="credit d-flex justify-content-center align-items-center gap-3">
            <img :src="img" alt="">
            <p class="text-light">{{whiteText}}</p>
            <p>{{text}}</p>
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
    padding: 0 1rem 3rem;
    margin: auto;

    h2 {
        color: white;
        font-weight: bold;
    }

    .credit {
        width: 100%;

        img {
            max-width: 40px;
            border-radius: 50%;
        }

        p {
            color: #bcbcbc;
            margin-bottom: 0;
        }
    }

    .element{
        margin-top: 1rem;
    }

}
</style>