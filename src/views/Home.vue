<template>
  <div class="home">
    <Crear/>
  </div>
</template>

<script>
// @ is an alias to /src
import Crear from '@/components/Crear.vue'
export default {
  name: 'Home',
  components: {
    Crear
  }
}
</script>
