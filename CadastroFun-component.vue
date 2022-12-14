<template>
    <div id="container">
    <form id="form">
        <div class="inputs">
            <label for="nome">Nome:</label>
            <input 
                type="text"
                id="nome"
                name="nome"
                v-model="nome"
                placeholder="Digite seu nome"
                required="">
        </div>
        <div class="inputs">
            <label for="Rg">Rg:</label>
            <input
                type="number"
                id="rg"
                name="rg"
                v-model="rg"
                placeholder="Digite seu RG"
                required>
        </div>
        <div class="inputs">
            <label for="E-mail">E-mail:</label>
            <input
                type="text"
                id="email"
                name="email"
                v-model="email"
                placeholder="Digite seu E-mail"
                required>
        </div>
        <div class="inputs">
            <label for="nome">Telefone:</label>
            <input
                type="text"
                id="nome"
                name="nome"
                v-model="telefone"
                placeholder="Digite seu Telefone"
                required>
        </div>
        <div class="inputs">
            <label for="Endereco">Endereço:</label>
            <input
                type="text"
                id="nome"
                name="nome"
                v-model="endereco"
                placeholder="Digite seu Endereço"
                required>
        </div>
        <div class="inputs">
            <label for="Foto">Foto:</label>
            <input type="file" id="file" accept="image/*">
        </div>
        <div class="submit">
            <input type="submit" value="Enviar">
        </div>
    </form>
    </div>
</template>
<script>
    export default {
        data() {
            return {
                nome: '',
                rg: '',
                email: '',
                telefone: '',
                endereco: '',
                foto: ''
            }
        }
    }
</script>
    
    <style scoped>
   #container{
    width: 460px;
    height: 550px;
    background-color: rgb(199, 209, 224);
    border-radius: 20px;
    position: absolute;
    top: 80px;
    bottom: 0;
    left: 0;
    right: 0;
    margin:auto;
    display: inline-block;
   
   }

   #form{
        max-width: 400px;
        margin: 0 auto;
    
    }
    .inputs{
        display: flex;
        flex-direction: column;
        margin-bottom: 10px;
       
        cursor: pointer;
    
    }
    .inputs:hover{
        opacity: .7;
        color:  rgb(199, 209, 224);
    }
    label{
        font-weight: bolder;
        margin-bottom: 15px;
        color: #222;
        padding: 5px 10px;
        border-left: 2px solid green;

    }
    .submit input{
    cursor: pointer;
    border: 2px solid #222;
    font-size: 16px;
    font-weight: bolder;
    padding: 10px;
    color: white;
    margin: 0 auto;
    border-radius: 10px;
    background-color: rgb(137, 197, 217);
    transition: .3s;
    }
    .submit input:hover{
        background-color: transparent ;
        color: #222;
    }
</style>