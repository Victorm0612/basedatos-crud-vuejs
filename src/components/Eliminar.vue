<template>
    <div class="container">
        <div class="abs-center flex-column">
            <h3 class="mb-3">Eliminar Paciente</h3>
            <form>
            <div class="form-group">
                <input placeholder="Digite el id" type="text" class="form-control" id="id" name="id">              
            </div>
            <button type="submit" class="mt-3 btn btn-danger">Eliminar</button>
            </form>  
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Eliminar'
    }
</script>

<style lang="sass" scoped>

</style>