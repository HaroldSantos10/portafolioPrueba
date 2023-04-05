<template>


    <section class="page-section" >

        <div class="container px-4 px-lg-5">
            <div class="row gx-4 gx-lg-5 justify-content-center ">
                <div class="col-lg-8 col-xl-6 text-center">
                            <h2 class="mt-0">Apuntes</h2>
                            <hr class="divider" />
                            <p class="text-muted mb-1">
                            En esta sección pueden encontrarse los apuntes tomados durante el desarrollo de las
                            clases, tanto prácticas como teóricas que fueron impartidas a lo largo de este computo.
                            </p>
                            <br>
                </div>
                
                <carousel :Slides="imagenes" ></carousel>

            </div>
        </div>
    </section>



  </template>
  
<script>

import carousel from '../components/carousel.vue';


export default({
    components:{
        carousel,
        
    },
    data: () => ({
        imagenes: [

            '/public/img/apuntes/img01.png',
            '/public/img/apuntes/img02.png',
            '/public/img/apuntes/img03.png',
            '/public/img/apuntes/img04.png',
            '/public/img/apuntes/img05.png',
            '/public/img/apuntes/img113.png',
            '/public/img/apuntes/img123.png',
            '/public/img/apuntes/img06.png',
            '/public/img/apuntes/img07.png',
            '/public/img/apuntes/img08.png',
            '/public/img/apuntes/img09.png',
            '/public/img/apuntes/img10.png',

            
        ]
    })
});


</script>
  