<template>
<div>
    <p>Componente de mensagens</p>
</div>
<div>
    <form id="burger-form">
        <div class="input-container">
            <label for="nome">Nome do cliente</label>
            <input type="text" id="nome" name="nome" v-model="nome" placeholder="Digite seu nome">
        </div>
        <div class="input-container">            
            <label for="pao">Escolha o pão</label>
            <select name="pao" id="pao" v-model="pao">
                <option value="">Selecione seu pão</option>
                <option value="integral">Integral</option>
            </select>           
        </div>
        <div class="input-container">            
            <label for="carne">Escolha o tipo de carne</label>
            <select name="carne" id="carne" v-model="carne">
                <option value="">Tipo de carne</option>
                <option value="integral">Bovina</option>
            </select>           
        </div>
        <div class="input-container">            
            <label for="opcionais">Selecione opcionais</label>
            <div class="checkbox-container">
                <input type="checkbox" name="opicionais" v-model="opcionais" value="salame">
                <span>Folhas</span>
            </div>
        </div>
        <div class="input-container">
            <input type="submit" class="submit-btn" value="Criar meu Burger">
        </div>
                      
    
    </form>
</div>

</template>

<script>
export default{
    name: 'BurgerForm',

}
</script>

<style scoped>
#burger-form{
    max-width: 400px;
    margin:0 auto;
}
.input-container{
    
    display: flex;
    flex-direction: column;
    margin-bottom: 20px;
    
}
label{
    font-weight: bold;
    margin-bottom: 15px;
    color: #222;
    padding: 5px 10px;
    border-left: 4px solid #FCBA03;
}
</style>
