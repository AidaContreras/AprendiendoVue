<template>
  <div class="about">
    <Prueba msg="Acerca de"></Prueba>

      <p>First name: {{ firstName }}</p>
      <p>Last name: {{ lastName }}</p>

      <Prueba
        first-name="firstName"
        last-name="lastName"
      ></Prueba>
    
  </div>
</template>

<script>
// @ is an alias to /src
import Prueba from '@/components/Prueba.vue'

export default {
  name: 'About',
    components: {
      Prueba
    }, 
    data() {
      return {
        firstName: '',
        lastName: ''
      }
    }
}

</script>

