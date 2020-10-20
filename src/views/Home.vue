<template>
  <div class="home">
    <Create/>
  </div>
</template>

<script>
// @ is an alias to /src
import Create from '@/components/Create.vue'
export default {
  name: 'Home',
  components: {
    Create
  }
}
</script>
