<template>
    <div class="primary-banner pb-5">
        <div class="container pt-3 pb-5">
            <div class="row gap-5">
                <div class="col crossfit">
                    <img src="../assets/img/sep-white.svg" class="separator-small">
                    <h3>Crossfit workout</h3>
                    <h5>Push your limits</h5>
                </div>
                <div class="col apparel">
                    <img src="../assets/img/sep-white.svg" class="separator-small">
                    <h3>New gym apparel</h3>
                    <h5>Look good, feel good</h5>
                </div>
                <div class="col training">
                    <img src="../assets/img/sep-white.svg" class="separator-small">
                    <h3>Team training</h3>
                    <h5>Find a partner</h5>
                </div>
            </div>
            <div class="mot col-65">
                <h2>"How you respond to the challenge in the second half will determine what you become after
                    the game, whether you are a winner or a loser."</h2>
                <img src="../assets/img/sep.svg" class="separator mt-4 mb-2">
                <div class="credit d-flex justify-content-center align-items-center gap-3">
                    <img src="../assets/img/avatar-1-2x.jpg" alt="">
                    <p class="text-light">Brad Johnson</p>
                    <p>Las Vegas</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.primary-banner {
    background: rgb(7, 23, 227);
    background: linear-gradient(167deg, rgba(7, 23, 227, 1) 0%, rgba(25, 21, 208, 1) 10%, rgba(210, 0, 11, 1) 100%);

    .row {
        transform: translateY(-20%);
        .col {
            aspect-ratio: 1/1;
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            border-radius: 0.5rem 0.5rem 3rem;
            text-align: left;
            padding: 1rem;
            display: flex;
            flex-direction: column;
            justify-content: end;

            img{
                margin-bottom: 1rem;
            }
            h3{
                color: white;
                font-weight: bold;
            }
            h5{
                color: #fff014;
                font-weight: bold;
            }
        }

        .crossfit {
            background-image: linear-gradient(transparent, rgba(0, 0, 0, 0.5)), url(../assets/img/service6-2x.jpg);
        }

        .apparel {
            background-image: linear-gradient(transparent, rgba(0, 0, 0, 0.5)), url(../assets/img/box1-2x.jpg);
        }

        .training {
            background-image: linear-gradient(transparent, rgba(0, 0, 0, 0.5)), url(../assets/img/box3-2x.jpg);
        }
    }

    .mot{
        padding: 0 1rem 3rem;
        margin: auto;

        h2{
            color: white;
            font-weight: bold;
        }

        .credit{
            width: 100%;

            img{
                max-width: 40px;
                border-radius: 50%;
            }

            p{
                color: #bcbcbc;
                margin-bottom: 0;
            }
        }

    }
}
</style>