<template>
 <form>
   <input type="text"
          class="form-control my-2"
          placeholder="Ingrese nombre"
          v-model="texto"
   >

   <p>
     {{texto}}
   </p>
 </form>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
  components: {
  },

  data() {
    return {
      texto: "",
    }
  },
}
</script>
