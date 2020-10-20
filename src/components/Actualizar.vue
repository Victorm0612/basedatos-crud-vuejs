<template>
    <div class="container">
        <div class="abs-center flex-column">
            <h3 class="mb-3">Actualizar Paciente</h3>
            <form>
            <div class="form-group">
                <input placeholder="Digite el id de la persona" type="text" class="form-control" id="id" name="id">              
            </div>
            <div class="form-group">
                <input placeholder="Digite el numid" type="text" class="form-control" id="numid" name="numid">              
            </div>
            <div class="form-group">
                <input placeholder="Digite el nombre" type="text" class="form-control" id="nombre" name="nombre">
            </div>
            <div class="form-froup">
                <input placeholder="Digite el apellido" type="text" class="form-control" id="apellido" name="apellido">
            </div>
            <button type="submit" class="mt-3 btn btn-primary">Actualizar</button>
            </form>  
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Actualizar'
    }
</script>