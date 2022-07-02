<template>
    <header class="d-flex align-items-center">
        <div class="container d-flex justify-content-between align-items-center">
            <img src="../assets/img/logo.png" alt="Avada Fitness Logo">
            <div class="menu-container d-flex gap-4 align-items-center">
                <ul class="d-flex list-unstyled align-items-center mb-0 gap-4">
                    <li v-for="item in menu" :key="item" v-html="item"></li>
                </ul>
                <button class="primary-btn small">Schedule a workout</button>
                <div class="icons d-flex gap-4">
                    <i class="fa fa-solid fa-cart-shopping"></i>
                    <i class="fa fa-solid fa-magnifying-glass"></i>
                </div>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    data(){
        return{
            menu: [
                "<span class='active'>Home</span>",
                "<span>Services</span>",
                "<span>About</span>",
                "<span>Videos</span>",
                "<span>Blog</span>",
                "<span class='new'>Store</span>"
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    header{
        z-index: 10;
        position: fixed;
        top: 0;
        left: 0;
        right: 0;
        background: var(--black);
        min-height: 60px;
        padding: 1.5rem;
        color: var(--light-grey);
    }

    li, i{
        cursor: pointer;
        &:hover{
            color: var(--dark-grey);
        }
    }
</style>