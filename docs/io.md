# 5. Operações de entrada e saída de dados

Como dito anteriormente, JavaScript não possui em si uma API para acesso a objetos do sistema operacional, posto que foi desenvolvida para operar sobre
objetos dos navegadores Web.

Não obstante, os navegadores implementam um objeto denominado console que é o terminal de linha de comandos do Navegador.  Este objeto, porém, não possui métodos para leitura do teclado, posto que este é um objeto do sistema operacional ao qual o motor JavaScript do navegador não tem acesso.  Assim, pode-se escrever na tela do console, mas não se pode ler dados inseridos pelo usuário no teclado.

A solução para este problema se dá por meio de bibliotecas nas implementações JavaScript para o sistema operacional.  Veremos como isso é feito no NodeJS.

## 5.1 Saída de dados na tela do terminal

Para realizar saída de dados na tela, use:

```javascript
let x = 2;
console.log(x);
```

## 5.2 Leitura de dados no teclado no NodeJS

O NodeJS implementa uma biblioteca-padrão contendo métodos para acesso ao teclado.  Assim, ele se mantém fielmente como uma implementação da linguagem JavaScript sem abrir mão da capacidade de operar sobre os objetos do sistema operacional que é característica de uma linguagem de programação de uso gera.

Assim, para realizar leitura de dados do teclado, use:

```javascript
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
