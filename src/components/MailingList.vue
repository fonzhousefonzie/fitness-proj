<template>
    <div class="section">
        <FadedBanner
            :bgImage="require('../assets/img/banner1-2x.jpg')"
            :h5="'Join our mailing list today'"
            :h1="'Insider offers & flash sales in your inbox every week.'"
            :first-element="input"
            :primary-button="primButton"
            :p1="'Curatibur non nulla sit amet nisl tempus convallis quis ac lectus dolor sit amet, consectetur adipiscing elit sed porttitor lectus.'"
        />
    </div>
</template>

<script>
import FadedBanner from './FadedBanner.vue'

export default {
    data(){
        return{
            input: '<input type="email" placeholder="Insert your email...*" class="col-65 me-4">',
            primButton: '<span style="padding: 0 3.7rem;">Subscribe</span>'
        }
    },
    components:{FadedBanner}
}
</script>

<style lang="scss" scoped>

</style>