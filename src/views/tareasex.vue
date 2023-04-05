<template>
    
    <section class="page-section" >

        <div class="container px-4 px-lg-5">
            <div class="row gx-4 gx-lg-5 justify-content-center ">
                <div class="col-lg-8 col-xl-6 text-center">
                            <h2 class="mt-0">Tareas Ex-aula</h2>
                            <hr class="divider" />
                            <p class="text-muted mb-1">
                            En esta sección puede encontrarse una pequeña descripción de las
                            tareas ex-aula realizadas hasta el momento.
                            </p>
                </div>

    
            </div>

            <dl><dt>Sitio web y asignación en parejas</dt><dd>
                    Esta tarea consistió en crear un sitio web que contuviera los Curriculums Vitae de los
                    integrantes del grupo de trabajo, al mismo tiempo a cada grupo se les asignó un ejercicio
                    en especifico el cual debían de desarrollar.

                    <br><br>

                    Posteriormente a esto, se subió el repositorio de trabajo a github y luego se hizo el deploy de 
                    este haciendo uso de GitHub Pages, el enlace obtenido se envió en un buzón de entrega. <br>
                    Despues de la entrega, la clase teórica se realizo la exposición del sitio web y asignación 
                    ante el resto de la clase y la Ingeniera encargadad de la Asignatura.



                </dd></dl>

            <br>
            <hr>
            
            <carousel :Slides="imagenes"></carousel>

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

    '/public/img/ex/asignacion.jpeg',
    '/public/img/ex/asignacion1.PNG',
    '/public/img/ex/asignacion2.PNG',
    '/public/img/ex/nota.jpeg',
    '/public/img/ex/portada2.jpeg',

    
],



})
});


</script>