<template>
    <div>
      <H1 type="text" id="titulo">Cadastrar</H1>
    </div>
    <div id="cubo">
      <input type="text" id="texto" placeholder="Nome da empresa" style="border: none; outline: none;">
      </div>
      <div id="cubo">
      <input type="text" id="texto" placeholder="CNPJ" style="border: none; outline: none;">
      </div>
      <div id="cubo">
      <input type="text" id="texto" placeholder="Nome do dono" style="border: none; outline: none;">
      </div>
      <div id="cubo2">
      <input type="text" id="texto" placeholder="Resumo sobre a empresa" style="border: none; outline: none;">
      </div>
  
  </template>
  
  <style scoped>
  #titulo {
   font-size: 5cap;
    color: #293C6C; 
    text-align: center;
    position: relative;
    z-index: 1; 
    font-family: 'PoetsenOne', sans-serif;
    font-weight: 800;
    left:3%;
    margin-bottom: 25vh;
    top: 100%;
  }
  #cubo {
    height: 15%;
    width: 80%;
    background-color: #D9D9D9;
    position: relative;
    left: 15%;
    margin-bottom: 15px; 
    bottom: 30%;
    
  }
  #cubo2 {
    height: 40%;
    width: 80%;
    background-color: #D9D9D9;
    position: relative;
    left: 15%;
    margin-bottom: 15px; 
    bottom: 30%;
   
  }
  #texto {
    font-size: medium;
    width: 80%; 
    background-color: #D9D9D9;
    color: #929292;
    position: relative;
    top: 30%;
    left: 8%;
  }
  
  .main-text {
  font-size: 26px; /* Tamanho maior */
  font-style: italic; /* Itálico */
  font-weight: black; /* Peso da fonte */
  color: #fff;
  font-family: 'Lato', sans-serif; /* Fonte Lato */
  margin-bottom: 5px; /* Margem inferior */
  margin-top: 40px; /* Margem superior */
}

.secondary-text {
  font-size: 18px; /* Tamanho menor */
  font-weight: bold; /* Negrito */
  color: #ccc;
  font-family: 'Lato', sans-serif; /* Fonte Lato */
  margin-bottom: 15px; /* Margem inferior */
}

.button.custom-button {
  width: 35%;
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
  margin: 20px auto; /* Centralizar verticalmente */
}

.button.custom-button:hover {
  background-color: #ffffff; 
  color: #000000; 
}

.button.custom-button:active {
  transform: scale(1.5);
}
  </style>
  
  
  