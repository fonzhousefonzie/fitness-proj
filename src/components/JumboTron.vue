<template>
    <div class="jumbotron">
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
        <div class="container py-5 text-start d-flex">
            <div class="col-65">
                <h5>Certified fitness professional</h5>
                <h1>Take control of your health</h1>
                <img src="../assets/img/sep.svg" class="separator my-4">
                <p class="mb-4">Curatibur non nulla sit amet nisl tempus convalis quis ac lectus dolor sit amet.</p>
                <button class="primary-btn fw-bold">
                    <i class="fa fa-brands fa-youtube"></i> Visit my YouTube channel
                </button>
                <button class="secondary-btn fw-bold ms-3">
                    Buy Avada today <i class="fa fa-solid fa-arrow-right"></i>
                </button>
            </div>
            <div class="col-30 d-flex justify-content-center align-items-center">
                <button class="play-btn"><i class="fa fa-solid fa-play"></i></button>
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.jumbotron {
    position: relative;
    margin-top: 86px;
    background: linear-gradient(90deg, #060606, #060606, rgba(0, 0, 0, 0.2), transparent), url(../assets/img/slider82x-scaled.jpg);
    background-position: center, top right;
    background-size: cover;
    background-repeat: no-repeat;
    color: #78787a;
    padding: 3rem 0 5rem;

    .col-65 {

        h5 {
            color: #ec5a57;
            font-weight: bold;
        }

        h1 {
            color: white;
            font-weight: bold;
        }
    }

    .col-30{
        width: 30%;
    }

    .absolute-buttons-container{
        position: absolute;
        right: 0.5rem;
        top: 1.5rem;

        .squared-button{
            background: white;
            color: #a00644;
            padding: 0.5rem;
            font-size: 0.6rem;
            font-weight: bold;
            margin-bottom: 0.5rem;
            width: 55px;
            height: 55px;
            border-radius: 0.3rem;
            cursor: pointer;
            transition: 200ms ease-out;

            img{
                max-width: 100%;
                margin: 0.2rem 0.5rem;
            }
            h4{
                font-weight: bold;
                color: #b6967e;
                margin-bottom: 0;
                span{
                    font-size: 1rem;
                    vertical-align: top;
                }
            }
            p{
                margin-bottom: 0;
            }

            &:hover{
                transform: scale(110%);
            }
        }
    }
}
</style>