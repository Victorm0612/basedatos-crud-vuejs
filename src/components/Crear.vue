<template>
    <div class="container">
        <div class="abs-center flex-column">
            <h3 class="mb-3">Crear Paciente</h3>
            <form>
            <div class="form-group">
                <input placeholder="Digite la identificación" type="text" class="form-control" id="numid" name="numid">              
            </div>
            <div class="form-group">
                <input placeholder="Digite el nombre" type="text" class="form-control" id="nombre" name="nombre">
            </div>
            <div class="form-froup">
                <input placeholder="Digite el apellido" type="text" class="form-control" id="apellido" name="apellido">
            </div>
            <button type="submit" class="mt-3 btn btn-primary">Guardar</button>
            </form>  
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Create'
    }
</script>
<style>
.abs-center {
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 100vh;
    width: auto;
    margin: auto;

}

.form {
    width: 50px;
    border: black;
}
</style>