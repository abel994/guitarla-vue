<script setup>

const props = defineProps({
    guitarra:{
        type:Object,
        require:true
    }
})

</script>

<template>
    <div v-for="guitarra in guitarras" class="col-md-6 col-lg-4 my-4 row align-items-center">
        <div class="col-4">
            <img class="img-fluid" src="/img/guitarra_01.jpg" alt="imagen guitarra">
        </div>
        <div class="col-8">
            <h3 class="text-black fs-4 fw-bold text-uppercase">{{ guitarra.nombre }}</h3>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Sit quae labore odit magnam in autem nesciunt, amet deserunt</p>
            <p class="fw-black text-primary fs-3">$299</p>
            <button 
                type="button"
                class="btn btn-dark w-100 "
            >Agregar al Carrito</button>
        </div>
    </div><!-- FIN GUITARRA -->
</template>

<style lang="scss" scoped>

</style>