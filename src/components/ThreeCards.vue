<template>
    <div class="container py-5">
        <div class="header d-flex justify-content-between fw-bold">
            <h6 class="fw-bold">{{title}}</h6>
            <a href="#">{{CTA}} <i class="fa fa-solid fa-angle-right"></i></a>
        </div>
        <div class="cards-container d-flex justify-content-between" :class="{'text-start' : textStart}">
            <div class="col-30">
                <div class="bg d-flex justify-content-center align-items-center" 
                :class="{'c-b-radius' : borderRadius}" 
                :style="{backgroundImage: 'url(' + bgFirst + ')'}">
                    <button class="play-btn small" :class="{'d-none' : noButton}"><i class="fa fa-solid fa-play"></i></button>
                </div>
                <h6 class="mx-3 fw-bold">{{firstTitle}}</h6>
                <p class="mx-3 subtitle" :class="{'blue-sub' : blueSubtitles}">{{firstSubtitle}}</p>
            </div>
            <div class="col-30">
                <div class="bg d-flex justify-content-center align-items-center" 
                :class="{'c-b-radius' : borderRadius}" 
                :style="{backgroundImage: 'url(' + bgSecond + ')'}">
                    <button class="play-btn small" :class="{'d-none' : noButton}"><i class="fa fa-solid fa-play"></i></button>
                </div>
                <h6 class="mx-3 fw-bold">{{secondTitle}}</h6>
                <p class="mx-3 subtitle" :class="{'blue-sub' : blueSubtitles}">{{secondSubtitle}}</p>
            </div>
            <div class="col-30">
                <div class="bg d-flex justify-content-center align-items-center" 
                :class="{'c-b-radius' : borderRadius}" 
                :style="{backgroundImage: 'url(' + bgThird + ')'}">
                    <button class="play-btn small" :class="{'d-none' : noButton}"><i class="fa fa-solid fa-play"></i></button>
                </div>
                <h6 class="mx-3 fw-bold">{{thirdTitle}}</h6>
                <p class="mx-3 subtitle" :class="{'blue-sub' : blueSubtitles}">{{thirdSubtitle}}</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props:{
        title: String,
        CTA: String,
        bgFirst: String, // to pass this prop you need to put the string in the require() function!!
        bgSecond: String, // to pass this prop you need to put the string in the require() function!!
        bgThird: String, // to pass this prop you need to put the string in the require() function!!
        borderRadius: Boolean,
        textStart: Boolean,
        firstTitle: String,
        firstSubtitle: String,
        secondTitle: String,
        secondSubtitle: String,
        thirdTitle: String,
        thirdSubtitle: String,
        blueSubtitles: Boolean,
        noButton: Boolean
    }
}
</script>

<style lang="scss" scoped>
    i{
        margin-left: 0.5rem;
    }
    .col-30{
        .bg{
        aspect-ratio: 3 / 2;
        width: 100%;
        background-size: cover;
        background-posizion: top center;
        margin: 1.5rem 0;
        }

        .blue-sub{
            color: var(--blue);
            font-weight: bold;
        }
    }
</style>