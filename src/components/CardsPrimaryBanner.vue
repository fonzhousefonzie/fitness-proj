<template>
    <div class="primary-banner">
        <div class="container pt-3 pb-5">
            <div class="row gap-5">
                <div class="col crossfit c-b-radius">
                    <img src="../assets/img/sep-white.svg" class="separator-small">
                    <h3>Crossfit workout</h3>
                    <h5>Push your limits</h5>
                </div>
                <div class="col apparel c-b-radius">
                    <img src="../assets/img/sep-white.svg" class="separator-small">
                    <h3>New gym apparel</h3>
                    <h5>Look good, feel good</h5>
                </div>
                <div class="col training c-b-radius">
                    <img src="../assets/img/sep-white.svg" class="separator-small">
                    <h3>Team training</h3>
                    <h5>Find a partner</h5>
                </div>
            </div>
            <H2Mot 
            :h2="quote" 
            :img="require('../assets/img/avatar-1-2x.jpg')" 
            :whiteText="'Brad Johnson'"
            :text="'Las Vegas'"
            />
        </div>
    </div>
</template>

<script>
import H2Mot from './H2Mot.vue';
export default {
    data(){
        return{
            quote: '"How you respond to the challenge in the second half will determine what you become after the game, whether you are a winner or a loser."'
        }
    },
    components: { H2Mot }
}
</script>

<style lang="scss" scoped>
.primary-banner {
    background: rgb(7, 23, 227);
    background: linear-gradient(167deg, rgba(7, 23, 227, 1) 0%, rgba(25, 21, 208, 1) 10%, rgba(210, 0, 11, 1) 100%);
    padding-bottom: 7rem;

    .row {
        transform: translateY(-20%);
        .col {
            aspect-ratio: 1/1;
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            text-align: left;
            padding: 2rem;
            display: flex;
            flex-direction: column;
            justify-content: end;
            cursor: pointer;
            box-shadow: 0 0.5rem 2rem rgba(0,0,0,0.3);
            transition: 300ms ease-out;
            &:hover{
                transform: scale(105%);
                box-shadow: 0 0.4rem 1.3rem rgba(0,0,0,0.5);
            }

            img{
                margin-bottom: 1rem;
            }
            h3{
                color: white;
                font-weight: bold;
            }
            h5{
                color: var(--yellow);
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
}
</style>