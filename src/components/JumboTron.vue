<template>
    <div class="section position-relative">
        <div class="absolute-buttons-container">
            <div class="squared-button">
                <img src="../assets/img/demos-icon.svg">
                <p>Demos</p>
            </div>
            <div class="squared-button">
                <h4><span>$</span>39</h4>
                <p>On Sale</p>
            </div>
        </div>
        <FadedBanner
        :bg-image="bgImg"
        :h5="'Certified fitness professional'"
        :h1="'Take control of your health'"
        :p="'Curatibur non nulla sit amet nisl tempus convalis quis ac lectus dolor sit amet.'"
        :primary-button="primButton"
        :second-element="secButton"
        :small-col-element="playButton"
        />
    </div>
</template>

<script>
import FadedBanner from "./FadedBanner.vue";
export default {
    data(){
        return{
            bgImg: require('../assets/img/slider82x-scaled.jpg'),
            primButton: '<i class="fa fa-brands fa-youtube"></i> Visit my YouTube channel',
            secButton: '<button class="secondary-btn fw-bold ms-3">Buy Avada today <i class="fa fa-solid fa-arrow-right"></i></button>',
            playButton: '<button class="play-btn"><i class="fa fa-solid fa-play"></i></button>'
        }
    },
    components: { FadedBanner }
}
</script>

<style lang="scss" scoped>
.section{
    padding-top: 86px;
}

.absolute-buttons-container {
    position: absolute;
    right: 1.5rem;
    top: calc(1.5rem + 86px);

    .squared-button {
        background: white;
        color: var(--darker);
        padding: 0.5rem;
        font-size: 0.6rem;
        font-weight: bold;
        margin-bottom: 0.5rem;
        width: 55px;
        height: 55px;
        border-radius: 0.3rem;
        cursor: pointer;
        transition: 200ms ease-out;

        img {
            max-width: 100%;
            margin: 0.2rem 0.5rem;
        }

        h4 {
            font-weight: bold;
            color: var(--lighter);
            margin-bottom: 0;

            span {
                font-size: 1rem;
                vertical-align: top;
            }
        }

        p {
            margin-bottom: 0;
        }

        &:hover {
            transform: scale(110%);
        }
    }
}
</style>