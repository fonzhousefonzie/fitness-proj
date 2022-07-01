<template>
    <footer>
        <div class="container py-5">
            <div class="row row-cols-3 g-3 py-5">
                <div class="col p-3">
                    <img src="../assets/img/logo.png" alt="Avada Fitness Logo">
                    <p class="py-5 mb-0">Ac aliquam neque sagittis diam faucibus vitae purus turpis phasellus. Pellentesque consectur amet purus ultrices mauris.</p>
                    <div class="social-icons">
                        <i class="fa fa-brands fa-facebook"></i>
                        <i class="fa fa-brands fa-twitter"></i>
                        <i class="fa fa-brands fa-youtube"></i>
                        <i class="fa fa-brands fa-instagram"></i>
                        <i class="fa fa-brands fa-linkedin"></i>
                    </div>
                </div>
                <div class="col p-3">
                    <h6 class="py-3">Recent Posts</h6>
                    <ul class="list-unstyled">
                        <li v-for="post in recentPosts" :key="post" class="py-2 posts"><i class="fa fa-solid fa-angle-right"></i> {{post}}</li>
                    </ul>
                </div>
                <div class="col p-3">
                    <h6 class="py-3">Contact Informations</h6>
                    <ul class="list-unstyled">
                        <li><span class="py-3">4748 Tipple Road Michigan 48449</span></li>
                        <li>Mobile:1.800.000.000</li>
                        <li>Email:info@your-company.com</li>
                    </ul>
                </div>
            </div>
        </div>
        <div class="copyright">
            <p>&copy;Copyright 2012 - 2020 | Avada Theme by <a href="#">ThemeFusion</a> | All rights reserved | Powered by <a href="#">Wordpress</a></p>
        </div>
    </footer>
</template>

<script>
export default {
    data(){
        return{
            recentPosts:[
                "The best protein shake",
                "Ultimate cardio workout",
                "New juices available now",
                "Tips to find training partners",
                "20 best healty recipes"
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
footer {
    background: #060606;
    color: white;
}

.social-icons i{
    color: #ec5a57;
    padding: 0 0.5rem;
    cursor: pointer;
    &:hover{
        color: #f78280;
        transform: scale(120%);
    }
}

h6{
    text-transform: uppercase;
}

.posts{
    cursor: pointer;
    &:hover{
        color: #bcbcbc;
    }
}

span{
    display: inline-block;
    color: #bcbcbc;
    cursor: pointer;
    &:hover{
        color: white;
    }
}

.copyright{
    color: #78787a;
    font-size: 0.8rem;
    padding: 2rem;
    border-top: 1px solid #78787a;
    p{
        padding: 0;
        margin: 0;
    }
    a{
        text-decoration: none;
        color: white;
    }
}
</style>