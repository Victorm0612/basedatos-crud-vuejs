<template>
    <div class="container">
        <div class="flex-column" id="tabla">
            <h3 class="mb-3">Leer Pacientes</h3>
            <button class="btn btn-danger mb-3" @click="leer">Consultar</button>
            <table class="table">
            <thead class="thead-dark">
                <tr>
                <th scope="col">ID</th>
                <th scope="col">Nombre</th>
                <th scope="col">Apellido</th>
                <th scope="col">Numid</th>
                </tr>
            </thead>
            <tbody id="contenido">
                <tr v-for="item of pacientes" :key="item.id">
                <th scope="row">{{item.id}}</th>
                <td>{{item.nombre}}</td>
                <td>{{item.apellido}}</td>
                <td>{{item.numid}}</td>
                </tr>
            </tbody>
            </table>
        </div>
    </div>
</template>

<script>
import axios from 'axios';
    export default {
        name: 'Leer',
        data(){
            return{
                pacientes: []
            }
        },
        methods: {
            leer(env){
                env.preventDefault();
                axios.get('consultatotalpacientes')
                    .then(res=>{
                        this.pacientes = res.data
                        console.log(this.pacientes)
                    })

            }
        },
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