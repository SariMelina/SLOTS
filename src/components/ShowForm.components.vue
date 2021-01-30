<template>
    <form class="form">       
        <slot name="titulo"/>
        <slot name="correo"/>
        <slot name="boton"/>        
    </form>
</template>

<script>
export default {

}
</script>

<style>
    h3{
        color: red;
    }
</style>