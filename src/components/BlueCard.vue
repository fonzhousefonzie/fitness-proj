<template>
    <div class="my-card col-30" :class="{'bordered' : bordered}">
        <img :src="img" alt="">
        <h5>{{title}}</h5>
        <h6>{{subtitle}}</h6>
        <p>{{text}}</p>
        <a href="#">{{link}} <i class="fa fa-solid fa-angle-right"></i></a>
    </div>
</template>

<script>
export default {
    props:{
        img: String,
        title: String,
        subtitle: String,
        text: String,
        link: String,
        bordered: Boolean
    }
}
</script>

<style lang="scss" scoped>
.bordered{
    cursor: pointer;
    border: 4px solid var(--blue);
    border-radius: 0.5rem;
    transition: 300ms ease-out;
    *{
        transition: 300ms ease-out;
    }
    &:hover{
        transform: scale(110%);
        *{
            transform: scale(92.5%);
        }
    }
}

.my-card {
    padding: 5rem 2rem;

    h5 {
        font-weight: bold;
        margin-top: 2rem;
    }

    h6{
        font-weight: bold;
        color: var(--yellow);
        margin-bottom: 3rem;
    }

    p{
        color: var(--light-grey);
        margin-bottom: 2rem;
    }

    a{
        font-weight: bold;
        i{
            padding-left: 0.5rem;
        }
    }

    img {
        max-height: 70px;
    }
}
</style>