<template>
   <div id="Prueba">

    <h1>{{ msg }}</h1>

    <input 
      type="text"
      v-model="firstName"
      @input="$emit('update:firstName', $event.target.value)">

    <input
      type="text"
      v-model="lastName"
      @input="$emit('update:lastName', $event.target.value)">

   </div>

</template>


<script>
export default {
  name: 'Prueba',
    props: {
        msg: String
    },
    data() {
      return {
        firstName: 'John',
        lastName: 'Doe',
      };
    }
}
</script>



