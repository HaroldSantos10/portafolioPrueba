<template >
    <!-- Navigation-->
        <nav class="navbar navbar-expand-lg navbar-light fixed-top py-3" id="mainNav">
            <div class="container px-4 px-lg-5">
                <a class="navbar-brand" href="/">{{brandName}}</a>
                <button class="navbar-toggler navbar-toggler-right" type="button" data-bs-toggle="collapse" data-bs-target="#navbarResponsive" aria-controls="navbarResponsive" aria-expanded="false" aria-label="Toggle navigation"><span class="navbar-toggler-icon"></span></button>
                <div class="collapse navbar-collapse" id="navbarResponsive">
                    <ul class="navbar-nav ms-auto my-2 my-lg-0">
                        <li class="nav-item" v-for="route in routes" :key="route">
                            <router-link :to="route.path" class="nav-link">{{route.name}}</router-link>
                        </li>
                    </ul>
                </div> 
            </div>
        </nav>
</template>
<script>
export default({
    props: {
        brandName: String
    },
    data(){
        return{
            routes: []
        }
    },
    created(){
        this.$router.options.routes.forEach(route => {
            this.routes.push({
                name: route.name,
                path: route.path
            })
        })
    }
})
</script>