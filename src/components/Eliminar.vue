<template>
    <div class="container">
        <div class="abs-center flex-column">
            <h3 class="mb-3">Eliminar Paciente</h3>
            <form>
            <div class="form-group">
                <input placeholder="Digite el id" type="text" class="form-control" v-model.number="id" name="id">              
            </div>
            <button type="submit" class="mt-3 btn btn-danger" @click="eliminar">Eliminar</button>
            <b-alert class="mt-3" 
                :show="show"
                dismissible
                variant="success"
                @dismissed="show=false">{{data}}
            </b-alert>
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
                id: '',
                data: '',
                show: false
            }
        },
        methods: {
            eliminar(evt){
                evt.preventDefault();
                axios.delete('borrarpacientes/'+this.id)
                .then(res =>{
                    this.data = JSON.stringify(res.data.RES);
                    this.show = !this.show;
                })
            }
        },
    }
</script>
