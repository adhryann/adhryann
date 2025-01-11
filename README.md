<!doctype html>
<html lang="pt-BR"> 
 <head> 
  <meta charset="UTF-8"> 
  <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
  <title>RenovaTech - Celulares Renovados</title> 
  <link rel="stylesheet" href="style.css"> 
 </head> 
 <body> 
  <header> 
   <div class="logo"> 
    <h1>RenovaTech</h1> 
   </div> 
   <nav> 
    <ul> 
     <li><a href="#sobre">Sobre</a></li> 
     <li><a href="#produtos">Produtos</a></li> 
     <li><a href="#contato">Contato</a></li> 
     <li><a href="#vender" id="vender-celular">💼 Vender Celular</a></li> 
     <li> <button id="carrinho">🛒 Carrinho</button> </li> 
    </ul> 
   </nav> 
  </header> 
  <main> 
   <section id="sobre"> 
    <h2>Sobre Nós</h2> 
    <p>A RenovaTech é especialista em assistência técnica e renovação de celulares. Aqui você encontra qualidade, garantia e preços acessíveis. Confiança e tecnologia ao seu alcance!</p> 
   </section> 
   <section id="produtos"> 
    <h2>Produtos Disponíveis</h2> 
    <div class="produto"> 
     <h3>iPhone X - 64GB</h3> 
     <p>R$ 2.000,00</p> <button class="adicionar-carrinho" data-produto="iPhone X - 64GB" data-preco="2000">Adicionar ao Carrinho</button> 
    </div> 
    <div class="produto"> 
     <h3>Samsung Galaxy S10</h3> 
     <p>R$ 1.500,00</p> <button class="adicionar-carrinho" data-produto="Samsung Galaxy S10" data-preco="1500">Adicionar ao Carrinho</button> 
    </div> 
    <div class="produto"> 
     <h3>Motorola G9</h3> 
     <p>R$ 1.000,00</p> <button class="adicionar-carrinho" data-produto="Motorola G9" data-preco="1000">Adicionar ao Carrinho</button> 
    </div> 
   </section> 
   <section id="vender"> 
    <h2>Vender seu Celular Usado</h2> 
    <p>Quer vender seu celular usado? Preencha o formulário abaixo e nossa equipe entrará em contato para oferecer a melhor proposta.</p> <a href="vender.html" class="btn-vender">Clique aqui para vender</a> 
   </section> 
  </main> 
  <footer> 
   <p>© 2025 - RenovaTech. Todos os direitos reservados.</p> 
  </footer> 
  <script src="script.js"></script> 
 </body>
</html>
/* Reset Básico */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Roboto', sans-serif;
    background: #f5f5f5;
    color: #333;
    margin: 0;
    padding: 0;
}

/* Cabeçalho */
header {
    background: linear-gradient(90deg, #4CAF50, #3E8E41);
    color: #fff;
    text-align: center;
    padding: 20px 0;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

header .logo h1 {
    font-size: 2.5rem;
    font-weight: bold;
}

/* Navegação */
nav ul {
    display: flex;
    justify-content: center;
    gap: 20px;
    list-style-type: none;
}

nav ul li {
    display: inline-block;
}

nav ul li a, #vender-celular {
    font-size: 1.2rem;
    color: #fff;
    text-decoration: none;
    transition: color 0.3s ease;
}

nav ul li a:hover, #vender-celular:hover {
    color: #ffcc99;
}

/* Seção Sobre */
#sobre {
    background: #fff;
    padding: 40px;
    text-align: center;
    margin-top: 40px;
    border-radius: 8px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
}

#sobre h2 {
    font-size: 2rem;
    color: #333;
    margin-bottom: 15px;
}

/* Seção Produtos */
#produtos {
    padding: 40px;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 30px;
    text-align: center;
}

.produto {
    background: #fff;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
}

.produto h3 {
    font-size: 1.5rem;
    color: #333;
}

.produto p {
    font-size: 1.2rem;
    color: #555;
    margin: 10px 0;
}

.adicionar-carrinho {
    background-color: #4CAF50;
    color: #fff;
    padding: 10px 15px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

.adicionar-carrinho:hover {
    background-color: #45a049;
}

/* Seção Vender Celular */
#vender {
    background: #f0f8ff;
    padding: 30px;
    text-align: center;
    margin-top: 40px;
    border-radius: 8px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
}

#vender h2 {
    font-size: 2rem;
    color: #333;
    margin-bottom: 15px;
}

#vender p {
    font-size: 1.2rem;
    color: #555;
    margin-bottom: 20px;
}

.btn-vender {
    display: inline-block;
    background-color: #4CAF50;
    color: #fff;
    padding: 15px 25px;
    font-size: 1.2rem;
    border-radius: 5px;
    text-decoration: none;
    transition: background-color 0.3s ease, transform 0.2s ease;
}

.btn-vender:hover {
    background-color: #45a049;
    transform: scale(1.05);
}

/* Formulário de Vender Celular */
form {
    display: flex;
    flex-direction: column;
    gap: 20px;
    align-items: center;
}

form input,
form select,
form button {
    width: 80%;
    max-width: 400px;
    padding: 12px;
    border: 1px solid #ddd;
    border-radius: 5px;
    font-size: 1rem;
    transition: border-color 0.3s ease, box-shadow 0.3s ease;
}

form input:focus,
form select:focus {
    border-color: #4CAF50;
    box-shadow: 0 0 5px rgba(76, 175, 80, 0.5);
    outline: none;
}

form button {
    background: #4CAF50;
    color: #fff;
    font-size: 1.2rem;
    font-weight: bold;
    padding: 15px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.3s ease, transform 0.2s ease;
}

form button:hover {
    background: #45a049;
    transform: scale(1.02);
}

/* Responsividade */
@media (max-width: 768px) {
    #produtos {
        grid-template-columns: 1fr 1fr;
    }

    #vender {
        padding: 20px;
    }

    #vender h2 {
        font-size: 1.8rem;
    }

    #vender p {
        font-size: 1rem;
    }

    form input,
    form select,
    form button {
        width: 100%;
    }
}