<template>
    <div class="section">
        <div class="container d-flex justify-content-between">
            <BlueCard 
                :img="require('../assets/img/sport-watch.svg')"
                :title="'Team training'"
                :subtitle="'Find a partner'"
                :text="defaultText1"
                :link="'Find a partner'"
                :bordered="true"
            />
            <BlueCard 
                :img="require('../assets/img/crossfit.svg')"
                :title="'Crossfit workout'"
                :subtitle="'Push your limits'"
                :text="defaultText1"
                :link="'Learn about Crossfit'"
                :bordered="true"
            />
            <BlueCard 
                :img="require('../assets/img/weight-loss.svg')"
                :title="'Weight loss plan'"
                :subtitle="'Shed those pounds'"
                :text="defaultText2"
                :link="'Schedule a workout'"
                :bordered="true"
            />
        </div>
    </div>
</template>

<script>
import BlueCard from './BlueCard.vue';
export default {
    data(){
        return{
            defaultText1: 'Vestibulum, curatibur eu sem nibh ultrices sit nulla adipiscing. Nisl sit fames amet senectus eget sed duis vehicula. Tristique.',
            defaultText2: 'At laoreet senectus volupat diam vel sed sed amet pellentesque. Lobortis ut aliquam risus purus. A tellus ut etiam.'
        }
    },
    components: { BlueCard }
}
</script>

<style lang="scss" scoped>
    .section{
        background: var(--black);
        color: white;
        padding: 5rem 0;
    }
</style>