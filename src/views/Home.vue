<template>
 <form>
   <input type="text"
          class="form-control my-2"
          placeholder="Ingrese nombre"
          v-model="tarea.nombre"
   >

    <div class="form-check form-check-inline">
      <input class="form-check-input" v-model="tarea.categorias" type="checkbox" id="inlineCheckbox1" value="javascript">
      <label class="form-check-label" for="inlineCheckbox1">Javascript</label>
    </div>
    <div class="form-check form-check-inline">
      <input class="form-check-input" v-model="tarea.categorias" type="checkbox" id="inlineCheckbox2" value="nodeJs">
      <label class="form-check-label" for="inlineCheckbox2">Node.js</label>
    </div>
 </form>

 <p>
   {{tarea}}
 </p>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
  components: {
  },

  data() {
    return {
      tarea: {
        nombre: "",
        categorias: [],
      }
    }
  },
}
</script>
