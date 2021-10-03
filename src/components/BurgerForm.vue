<template>
    <div>
        <p>component de mensagem</p>
        <div>
            <form id="burger-form">
                <div class="input-container">
                    <label for="name">Nome do Cliente:</label>
                    <input type="text" id="name" name="name" v-model="name" placeholder="Digite seu nome">
                </div>
                <div class="input-container">
                    <label for="pao">Escohla o pão:</label>
                    <select name="pao" id="pao" v-model="pao">
                        <option value="">Selecione seu pão</option>
                        <option value="">Integral</option>
                    </select>
                </div>
                <div class="input-container">
                    <label for="carne">Escohla a carne:</label>
                    <select name="carne" id="carne" v-model="carne">
                        <option value="">Selecione o tipo de carne</option>
                        <option value="">Picanha</option>
                    </select>
                </div>
                <div id="options-container" class="input-container">
                    <label id="options-title" for="options">Selecione os opcionais:</label>
                    <div class="checkbox-container">
                        <input type="checkbox" name="options" id="options" v-model="options" value="options">
                        <span>Salame</span>
                    </div>
                </div>
                <div class="input-container">
                    <input type="submit" class="submit-btn" value="Criar meu Buger!">
                </div>
            </form>
        </div>
    </div>
</template>
<script>
export default {
    name: "BurgerForm"
}
</script>

<style scoped>
#burger-form {
    max-width: 400px;
    margin: 0 auto;
}
.input-container {
    display: flex;
    flex-direction: column;
    margin-bottom: 20px;
}
label {
    font-weight: bold;
    margin-bottom: 15px;
    color: #222;
    padding: 5px 10px;
    border-left: 4px solid #FCBA03;
}
input, select {
    padding: 5px 10px;
    width: 300px;
}
#options-container{
    flex-direction: row;
    flex-wrap: wrap; 
}
#options-title {
    width: 100%;
}
.checkbox-container {
    display: flex;
    align-items: flex-start;
    width: 60%;
}
.checkbox-container span,
.checkbox-container input {
    width: auto;
}
.checkbox-container span {
    margin-left: 6px;
    font-weight: bold;
}
.submit-btn {
    width: 100%;
    background-color: #222;
    color: #FCBA03;
    font-weight: bold;
    border: 2px solid #222;
    padding: 16px;
    margin: 0 auto;
    cursor: pointer;
    transition: .5s;
}
.submit-btn:hover {
    background-color: transparent;
    color: #222;
}
</style>