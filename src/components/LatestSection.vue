<template>
    <div class="section">
        <ThreeCards
        :title="'Latest articles'"
        :c-t-a="'Read all articles'"
        :border-radius="false"
        :no-button="true"
        :text-start="true"
        :bg-first="firstBg"
        :first-title="'The best protein shake'"
        :first-subtitle="'By admin | November 26th,2019 | Gym'"
        :bg-second="secondBg"
        :second-title="'Ultimate cardio workout'"
        :second-subtitle="'By admin | November 26th,2019 | Gym'"
        :bg-third="thirdBg"
        :third-title="'New juices available now'"
        :third-subtitle="'By admin | November 26th,2019 | Gym'"
        />
    </div>
</template>

<script>
import ThreeCards from './ThreeCards.vue';
export default {
    data(){
        return{
            firstBg: require('../assets/img/blog4-2x.jpg'),
            secondBg: require('../assets/img/blog1-2x.jpg'),
            thirdBg: require('../assets/img/blog3-2x.jpg')
        }
    },
    components: { ThreeCards }
}
</script>

<style lang="scss" scoped>
    .section{
        padding: 5rem 0;
    }
</style>le