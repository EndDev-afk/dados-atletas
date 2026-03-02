🏆 Projeto de Certificação 2 – Dados dos Atletas

📌 Sobre o Projeto:

Este projeto consiste na criação de uma aplicação em JavaScript capaz de:

Receber informações de um atleta
Calcular sua categoria
Calcular seu IMC
Calcular sua média válida com base nas notas
Exibir todas as informações no console

A aplicação foi desenvolvida utilizando Programação Orientada a Objetos (POO) com a criação da classe Atleta.

================= 🚀 Tecnologias Utilizadas =========================

JavaScript (ES6+)

Node.js (execução no terminal)

================== 🧠 Conceitos Aplicados ===========================

Classes;
Métodos;
Construtor;
Arrays;

Ordenação (sort)

Métodos de array (shift, pop, reduce)

Estruturas condicionais (if / else)

Encapsulamento de dados

================== 📂 Estrutura da Classe ==========================

A classe Atleta possui os seguintes atributos:

nome;
idade;
peso;
altura;
notas;

🔹 Métodos de Cálculo

calculaCategoria()

calculaIMC()

calculaMediaValida()

🔹 Métodos Getters

obtemNomeAtleta()

obtemIdadeAtleta()

obtemPesoAtleta()

obtemAlturaAtleta()

obtemNotasAtleta()

obtemCategoria()

obtemIMC()

obtemMediaValida()

================ 📏 Regras de Negócio ==================================
🥇 Categoria por Idade
Idade	Categoria:

9 a 11	"Infantil";
12 a 13	"Juvenil";
14 a 15	"Intermediário";
16 a 30	"Adulto";
Demais	"Sem categoria";

================ ⚖️ Cálculo do IMC =====================================

Fórmula utilizada:
IMC = peso / (altura * altura)

================ 📊 Cálculo da Média Válida ============================

Metodologia:

Ordenar as notas em ordem crescente

Remover a menor nota

Remover a maior nota

Calcular a média das notas restantes

================ 💻 Exemplo de Uso =====================================

const atleta = new Atleta(
    "Cesar Abascal",
    30,
    80,
    1.70,
    [10, 9.34, 8.42, 10, 7.88]
);

console.log("Nome:", atleta.obtemNomeAtleta());
console.log("Idade:", atleta.obtemIdadeAtleta());
console.log("Peso:", atleta.obtemPesoAtleta());
console.log("Altura:", atleta.obtemAlturaAtleta());
console.log("Notas:", atleta.obtemNotasAtleta().join(","));
console.log("Categoria:", atleta.obtemCategoria());
console.log("IMC:", atleta.obtemIMC());
console.log("Média válida:", atleta.obtemMediaValida());

======================= Exemplos de Saída =============================

Nome: Cesar Abascal,
Idade: 30,
Peso: 80,
Altura: 1.7,
Notas: 10,9.34,8.42,10,7.88,
Categoria: Adulto,
IMC: 27.68166089965398,
Média válida: 9.253333333333334,
