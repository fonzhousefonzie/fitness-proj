<template>
    <div class="section">
        <div class="d-flex">
            <div class="col-50 c-b-radius">
                <button class="play-btn"><i class="fa fa-solid fa-play"></i></button>
            </div>
            <div class="col-50 right text-start">
                <h5>Tune up your workouts</h5>
                <h1 class="pb-4">The best health &amp; fitness advice online</h1>
                <a href="https://www.youtube.com/c/ThemeFusionVideos" target="blank" class="youtube-channel d-flex">
                    <img src="../assets/img/unnamed.jpg" alt="ThemeFusion Logo">
                    <div>
                        <p class="yt-name">ThemeFusion</p>
                        <div class="yt-subs d-flex">
                            <span><i class="fa fa-brands fa-youtube"></i>YouTube</span>
                            <span>999+</span>
                        </div>
                    </div>
                </a>
                <h6>Arcu eu facilisi ut quisque placerat nunc habitant. Magna semper mauris, venenatis, leo integer sit
                    pellentesque.</h6>
                <button class="tertiary-btn"><i class="fa fa-brands fa-youtube"></i>Visit my YouTube channel</button>
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.section {

    .right {
        padding: 7rem;

        h5 {
            color: var(--blue);
            font-weight: bold;
            padding: 2rem 0;
        }

        h6 {
            color: var(--dark-grey);
            padding: 2rem 0;
        }

        .youtube-channel {
            font-size: 0.8rem;
            text-decoration: none;
            color: black;

            img{
                margin: 0 0.5rem 0 0;
            }

            .yt-name {
                margin-bottom: 0;
            }

            .yt-subs {
                border: 1px solid var(--light-grey);

                span {
                    padding: 0.1rem 0.3rem;
                }

                span:first-child {
                    color: white;
                    background: red;
                    font-weight: bold;

                    i {
                        margin-right: 0.3rem;
                    }
                }
            }
        }

        button i{
            margin-right: 0.5rem;
        }
    }

    .c-b-radius {
        display: flex;
        justify-content: center;
        align-items: center;
        aspect-ratio: 1 / 1;
        background: linear-gradient(transparent, rgba(0, 0, 0, 0.3)), url(../assets/img/service15-2x.jpg);
        background-size: cover;
        background-position: top center;
        background-repeat: no-repeat;
        transform: translateY(-10%);
    }
}
</style>