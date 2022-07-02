<template>
    <div class="section">
        <ThreeCards
            :title="'Featured playlists'"
            :c-t-a="'View all videos'"
            :bg-first="bgFirst"
            :bg-second="bgSecond"
            :bg-third="bgThird"
            :border-radius="true"
            :first-title="'Thighs & glute workout'"
            :first-subtitle="'Increase your mobility'"
            :second-title="'Lift, firm & perk up'"
            :second-subtitle="'Feel young again'"
            :third-title="'Slim & trim yout waist'"
            :third-subtitle="'Shed those extra pounds'"
            :blue-subtitles="true"
        />
    </div>
</template>

<script>
import ThreeCards from './ThreeCards.vue'

export default {
    data(){
        return{
            bgFirst: require('../assets/img/video2-2x.jpg'),
            bgSecond: require('../assets/img/video7-2x.jpg'),
            bgThird: require('../assets/img/video9-2x.jpg')
        }
    },
    components:{ ThreeCards }
}
</script>

<style lang="scss" scoped>
    .section{
        padding-bottom: 5rem;
    }
</style>