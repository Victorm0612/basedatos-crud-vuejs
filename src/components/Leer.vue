<template>
    <div class="container">
        <div class="flex-column" id="tabla">
            <h3 class="mb-3">Leer Pacientes</h3>
            <table class="table">
            <thead class="thead-dark">
                <tr>
                <th scope="col">ID</th>
                <th scope="col">Nombre</th>
                <th scope="col">Apellido</th>
                <th scope="col">Numid</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                <th scope="row">1</th>
                <td>Mark</td>
                <td>Otto</td>
                <td>@mdo</td>
                </tr>
            </tbody>
            </table>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Leer'
        
    }
</script>

<style scoped>
#tabla {
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 100vh;
    width: auto;
    margin: auto;

}
</style>