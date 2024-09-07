
# Introdução à linguagem JavaScript

## 1. Características da linguagem: código-fonte, escopo, gestão de memória e implementações
JavaScript é uma linguagem de programação que suporta aos paradigmas sequencial, estruturado, procedural, funcional e orientado a objetos.  O código fonte JavaScript deve
ser inserido em um arquivo de texto de sistema operacional com extensão .js, ou seja, um programa nomeado hello teria seu código-fonte em um arquivo nomeado hello.js.
Ademais, o código-fonte é dividido em dois trechos: trecho de escopo global e trecho de escopo local. O trecho de escopo global manipula os objetos da linguagem que
serão armazenados em memória durante todo o tempo de execução do programa ao passo que o trecho de escopo local contém objetos que durarão apenas enquanto este trecho de
código estiver sendo executado.

A gestão de memória é automatizada pela implementação da linguagem a qual é responsável por organizá-la de acordo com os escopos previstos no código-fonte. 
A respeito das várias implementações de JavaScript, vale notar que inicialmente a linguagem se destinava apenas a automatizar procedimentos dentro do navegador Web NetScape
Navigator, sendo, posteriormente, adotada por todos os mais usados navegadores.  Atualmente, há também implementações para computadores Desktop (Node.JS e Deno.JS) e 
para dispositivos embarcados.

A fim de aprender JavaScript sem ter a necessidade de conhecer o ambiente Web (incluindo HTML e CSS), utilizaremos aqui a implementação [Node.JS](https://nodejs.org/en)
para exemplificar nossos códigos.  

## 2. Léxico
Utilizam-se os caracteres UTF-8 para denotar os objetos da semântica da linguagem.  Individualmente, cada caracter é chamado de literal da linguagem. Em particular,
os seguintes símbolos são especialmente importantes:

// - denota comentário de linha única
/* */ - denota comentário de múltiplas linhas
#! - é um símbolo chamado de comentário hashbang que funciona como comentário de linha única, mas só pode ser usado no início do programa

_ - Separadores numéricos.  Exemplo: 1_000_000 

## 3. Objetos e tipos de dados em JavaScript
Os dados manipulados por programas JavaScript são armazenados em objetos classificados de acordo com o tipo de dado onde se entende um tipo de dado como sendo o conjunto
ao qual pertece o dado armazenado acompanhado das operações que podem ser realizadas com dados deste conjunto.

Os tipos de dados JavaScript são dinâmicos, isto é, uma variável pode assumir um valor de um tipo em uma parte do programa e mudar de tipo em outra parte.  Além disso, os
tipos são fracos, ou seja, a implementação da linguagem vai buscar efetuar conversões de tipos em tempo de execução de tal modo a viabilizar uma operação em vez de
simplesmente retornar uma mensagem de erro.  Infelizmente, de modo geral, tipos dinâmicos e simultaneamente fracos em linguagens de alto nível tendem a gerar códigos-fonte
com bugs difíceis de rastrear ou entender.  Mas JavaScript não está sozinha nisso: também as linguagens PHP e R sofrem com tal deficiência.

Feitas estas considerações iniciais, vamos ao ponto da seção que é apresentar os tipos primitivos em JavaScript, que são:

- Boolean: serve para armazenar os valores lógicos true e false.
- Number: serve para armazenar  inteiros (mas não inteiros muito grandes) e números de ponto flutuante.
- String: serve para armazenar texto.
- BigInt: serve para armazenar  inteiros muito grandes.
- Symbol: serve para armazenar criar identificadores que não coincidem.
- Undefined: serve para indicar que uma variável não foi atribuída.
- Null: serve para indicar que a variável que recebe este tipo não possui valor.

Além dos tipos primitivos, JavaScript conta também com estruturas de dados denominadas simplesmente de objetos as quais, entre as mais importantes podemos citar as seguintes:
- Array
- Date
- Error
- Function

## 4. Variáveis
Variáveis são identificadores de endereços de memória onde são alocados os objetos (tipos primitivos ou objetos propriamente ditos) os quais são gerenciados pela implementação da linguagem.

A sintaxe para atribuição de variáveis também chamada de instanciamento de objetos é a seguinte:

- Para variáveis globais cujo valor pode mudar ao longo do código, use:

```
var identificador = valor;
```

ou 
```
var identificador; (o valor é undefined)
```


- Para variáveis locais cujo valor pode mudar ao longo do código, use:

```
let identificador = valor;
```

ou 
```
let identificador; (o valor é undefined)
```

- Para definir constantes locais, use:

```
const identificador = valor;
```
 
## 5. Operações de entrada e saída de dados
Para realizar saída de dados na tela, use:

```
let x = 2;
console.log(x);
```

Para realizar leitura de dados do teclado, use:

```
const readline = require('node:readline'); // importa o módulo readline


const rl = readline.createInterface({

  input: process.stdin,
  
  output: process.stdout,
  
});


rl.question(`Qual o seu nome?`, nome => {

  console.log(\n);
  
  rl.close();
  
});

```
