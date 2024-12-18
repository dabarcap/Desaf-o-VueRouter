<template lang="">
    <h1>Vista de Productos</h1> 
    
    <div class="row">
        <!-- primera -->
        <div class="col-sm-4 col-12 px-5 mb-4">
            <div class="card">
                <img src="./assets/img/colaciones.jpg" class="card-img-top" alt="colaciones"/>
                <div class="card-body">
                    <h5 class="card-title fw-bold">{{producto.nombre}}</h5>
                    <p class="card-text">{{producto.descripcion}}</p>
                </div>
                <ul class="list-group list-group-flush">
                    <li class="list-group-item">Precio: {{producto.precio}}</li>
                    <li class="list-group-item">Cantidad: {{producto.cantidad}}</li>
                </ul>
                <div class="card-body">
                    <a href="#" class="card-link">ver más</a>
                    <a href="#" class="card-link">comprar</a>
                </div>
            </div>
        </div>
    </div>

    <div>
        <router-link class="btn btn-success" to="/">Volver al inicio</router-link>
    </div>
</template>

<script>
export default {
  props: ["producto"],
};
</script>
