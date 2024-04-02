<template>
  <div>
    <H1 type="text" id="titulo">Criar conta</H1>
  </div>
  <div id="cubo">
    <input type="text" id="texto" placeholder="Nome" style="border: none; outline: none;">
    </div>
    <div id="cubo">
    <input type="text" id="texto" placeholder="Email" style="border: none; outline: none;">
    </div>
    <div id="cubo">
    <input type="text" id="texto" placeholder="Senha" style="border: none; outline: none;">
    </div>
    <button class="custom-button">CADASTRAR</button>

</template>

<style scoped>
#titulo {
 font-size: 5cap;
  color: #615874; 
  text-align: center;
  position: relative;
  z-index: 1; 
  font-family: 'PoetsenOne', sans-serif;
  font-weight: 800;
  left:3%;
  margin-bottom: 25vh;
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
#texto {
  font-size: medium;
  width: 80%; 
  background-color: #D9D9D9;
  color: #929292;
  position: relative;
  top: 30%;
  left: 8%;
}


.custom-button {
  background-color: #615874;
  border: 2px solid #615874; 
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
</style>



<!-- 
/* .item {
  
  margin-top: 2rem;
  display: flex;
  position: relative;
}

.details {
  flex: 1;
  margin-left: 1rem;
}

i {
  display: flex;
  place-items: center;
  place-content: center;
  width: 32px;
  height: 32px;

  color: var(--color-text);
}

h3 {
  font-size: 1.2rem;
  font-weight: 500;
  margin-bottom: 0.4rem;
  color: var(--color-heading);
}

@media (min-width: 1024px) {
  .item {
    margin-top: 0;
    padding: 0.4rem 0 1rem calc(var(--section-gap) / 2);
  }

  i {
    top: calc(50% - 25px);
    left: -26px;
    position: absolute;
    border: 1px solid var(--color-border);
    background: var(--color-background);
    border-radius: 8px;
    width: 50px;
    height: 50px;
  }

  .item:before {
    content: ' ';
    border-left: 1px solid var(--color-border);
    position: absolute;
    left: 0;
    bottom: calc(50% + 25px);
    height: calc(50% - 25px);
  }

  .item:after {
    content: ' ';
    border-left: 1px solid var(--color-border);
    position: absolute;
    left: 0;
    top: calc(50% + 25px);
    height: calc(50% - 25px);
  }

  .item:first-of-type:before {
    display: none;
  }

  .item:last-of-type:after {
    display: none;
  }
} */ -->