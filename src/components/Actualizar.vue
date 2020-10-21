<template>
    <div class="container">
        <div class="abs-center flex-column">
            <h3 class="mb-3">Actualizar Paciente</h3>
            <form>
            <div class="form-group">
                <input placeholder="Digite la id" type="text" class="form-control" v-model="id" name="id">              
            </div>
            <div class="form-group">
                <input placeholder="Digite el numid" type="text" class="form-control" v-model="numid" name="numid">              
            </div>
            <div class="form-group">
                <input placeholder="Digite el nombre" type="text" class="form-control" v-model="nombre" name="nombre">
            </div>
            <div class="form-froup">
                <input placeholder="Digite el apellido" type="text" class="form-control" v-model="apellido" name="apellido">
            </div>
            <button type="submit" class="mt-3 btn btn-primary" @click="enviar">Actualizar</button>
            </form>  
        </div>
    </div>
</template>

<script>
import axios from 'axios';
    export default {
        name: 'Actualizar',
        data() {
            return {
                id: '',
                nombre: '',
                apellido: '',
                numid: ''
            }
        },
        methods: {
            enviar(evt){
                evt.preventDefault();
                axios.put('actualizarpacientes',{
                    id: this.id,
                    nombre: this.nombre,
                    apellido: this.apellido,
                    numid: this.numid
                })
                .then(res => console.log(res.data))
            }
        },
    }
</script>