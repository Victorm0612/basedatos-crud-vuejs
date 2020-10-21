<template>
    <div class="container">
        <div class="abs-center flex-column">
            <h3 class="mb-3">Eliminar Paciente</h3>
            <form>
            <div class="form-group">
                <input placeholder="Digite el id" type="text" class="form-control" v-model.number="id" name="id">              
            </div>
            <button type="submit" class="mt-3 btn btn-danger" @click="eliminar">Eliminar</button>
            </form>  
        </div>
    </div>
</template>

<script>
import axios from 'axios';
    export default {
        name: 'Eliminar',
        data() {
            return {
                id: ''
            }
        },
        methods: {
            eliminar(evt){
                evt.preventDefault();
                axios.delete('borrarpacientes/'+this.id)
                .then(res => console.log(res.data))
            }
        },
    }
</script>
