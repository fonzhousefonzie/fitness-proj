<template>
    <div class="jumbotron" :style="{backgroundImage: 'url(' + bgImage + ')'}">
        <div class="container text-start d-flex">
            <div class="col-65">
                <h5>{{h5}}</h5>
                <h1>{{h1}}</h1>
                <img src="../assets/img/sep.svg" class="separator my-4">
                <h6 class="mb-4">{{p}}</h6>
                <span v-html="firstElement"></span>
                <button class="primary-btn fw-bold" v-html="primaryButton">
                </button>
                <span v-html="secondElement"></span>
            </div>
            <div class="col-30 d-flex justify-content-center align-items-center" v-html="smallColElement">
                
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props:{
        bgImage: String, //to pass this prop you need to put the string in the require() function!!
        h5: String,
        h1: String,
        p: String,
        firstElement: Element,
        primaryButton: Element,
        secondElement: Element,
        smallColElement: Element
    }
}
</script>

<style lang="scss" scoped>
.jumbotron {
    background-position: top right;
    background-size: cover;
    background-repeat: no-repeat;


    .col-65 {
        padding: 6rem 0 12rem;
        background: linear-gradient(90deg, #060606 65%, transparent);
        color: var(--dark-grey);

        h5 {
            color: var(--red);
            font-weight: bold;
        }

        h1 {
            color: white;
        }
    }

    .col-30 {
        width: 30%;
    }
}
</style>