<template>
 <FormCadastro />
 <CadastroFunComponent />
</template>

<script>
import CadastroFunComponent from './components/CadastroFun-component.vue';
import  FormCadastro from './components/FormCadastro.vue'

export default {
  name: 'App',
  components: {
    FormCadastro,
    CadastroFunComponent
}
}

</script>

<style>
body{
  background-color: rgb(255, 255, 255);
}
*{
  margin:0;
  padding:0;
}
</style>
