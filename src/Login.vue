<script setup lang="ts">
import BemVindo from './components/Login/BemVindo.vue';
import CriarEmpresa from  './components/Login/CriarEmpresa.vue';
import TheWelcome from './components/Login/ExCriarConta.vue';
import CadastrarEmpresa from './components/Login/CadastrarEmpresa.vue';



import { ref } from 'vue';
const mostrarPrimeiros = ref(true);
const inverterMostrarPrimeiros = () => {
  mostrarPrimeiros.value = !mostrarPrimeiros.value;
};

</script>

<template>
  <header v-if="!mostrarPrimeiros">
    <div class="wrapper">
      <CriarEmpresa msg2="Criar empresa" />
    </div>
  </header>

  <main v-if="!mostrarPrimeiros">
    <CadastrarEmpresa />
    <button class="custom-button" @click="inverterMostrarPrimeiros">VOLTAR</button>
  </main>

  <header v-if="mostrarPrimeiros">
    <div class="wrapper">
      <BemVindo msg="Bem vindo" />
    </div>
  </header>

  <main v-if="mostrarPrimeiros">
    <TheWelcome />
    <button class="custom-button" @click="inverterMostrarPrimeiros">CADASTRAR</button>
  </main>

  
</template>

<style scoped>
header {
  line-height: 1.5;
  
}
.logo {
  display: block;
  margin: 0 auto 2rem;
}

.custom-button {
  background-color: #293C6C;
  border: 2px solid #293C6C; 
  border-radius: 20px; 
  color: #ffffff; 
  padding: 10px 20px; 
  font-weight: bold;
  font-size: 1.6rem;
  text-transform: uppercase; 
  cursor: pointer; 
  transition: background-color 0.3s, color 0.3s; 
  position: relative;
  margin: 0 10px;
  margin: 20px; 
  margin-left: auto; 
  margin-right: auto; 
  left: 37%;
  bottom: 30%;
}

.custom-button:hover {
  background-color: #ffffff; 
  color: #000000; 
}

.custom-button:active {
  transform: scale(0.95);
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
