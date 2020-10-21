<template>
    <div class="container">
        <div class="abs-center flex-column">
            <h3 class="mb-3">Crear Paciente</h3>
            <form>
            <div class="form-group">
                <input placeholder="Digite la identificación" type="text" class="form-control" v-model="numid" name="numid">              
            </div>
            <div class="form-group">
                <input placeholder="Digite el nombre" type="text" class="form-control" v-model="nombre" name="nombre">
            </div>
            <div class="form-froup">
                <input placeholder="Digite el apellido" type="text" class="form-control" v-model="apellido" name="apellido">
            </div>
            <button type="submit" class="mt-3 btn btn-primary" @click="enviar">Guardar</button>
            </form>
            <b-alert class="mt-3" 
                :show="show"
                dismissible
                variant="success"
                @dismissed="show=false">{{data}}
            </b-alert>
        </div>
    </div>
</template>

<script>
import axios from 'axios';
    export default {
        name: 'Create',
        data(){
            return{
                show: false,
                nombre: '',
                apellido: '',
                numid: '',
                data: ''
            }
        },
        methods: {
            enviar(evt){
                evt.preventDefault();
                axios.post('insertarpaciente',{
                    nombre: this.nombre,
                    apellido: this.apellido,
                    numid: this.numid
                })
                .then(res => {
                    this.data = JSON.stringify(res.data.RES);
                    this.show = !this.show;
                })
            }
        },
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