<template>
  <HeaderComponent></HeaderComponent>
  <NavComponent></NavComponent>
  <router-view/>
</template>

<script>

import HeaderComponent from '@/components/HeaderComponent.vue'
import NavComponent from '@/components/NavComponent.vue'

export default{
  components:{
    NavComponent,
    HeaderComponent
  },
  created() {
    // Redirigir a la ruta de inventario al iniciar la aplicación
    this.$router.push({ name: 'inventario' });
  }
}
</script>
<style>
* {
  font-family: 'Montserrat', sans-serif;
  margin: 0;
  padding: 0;

}
  #app {
    font-family: 'Montserrat';
    margin: 0;
    padding: 0;
  }
</style>
