# 1. Características da linguagem: código-fonte, escopo, gestão de memória e implementações

JavaScript é uma linguagem de programação que suporta aos paradigmas sequencial, estruturado, procedural, funcional e orientado a objetos.  Em JavaScript, a menos dos tipos primitivos que serão especificados mais a frente, tudo é objeto, inclusive todo o ambiente de execução.

O código fonte JavaScript deve
ser inserido em um arquivo de texto de sistema operacional com extensão .js, ou seja, um programa nomeado hello teria seu código-fonte em um arquivo nomeado hello.js.

Faça isso agora!  Abra o editor de textos do seu sistema operacional e crie um arquivo com nome hello.js.

Ademais, o código-fonte é dividido em dois trechos: trecho de escopo global e trecho de escopo local.

O trecho de escopo global é aquele que se encontra fora de qualquer outro objeto, tais como, funções ou classes bem como todos os objetos definidos explicitamente para estar no escopo global por meio de sintaxe específica mostrada na página [Variáveis](variaveis.md).  O escopo global manipula os objetos da linguagem que
serão armazenados em memória durante todo o tempo de execução do programa.

Por outro lado, o trecho de escopo local é definido internamente a objetos, sendo formado por outros objetos que durarão apenas enquanto este trecho de
código estiver sendo executado.

Digite no arquivo hello.js o seguinte código:

```javascript
console.log("Hello, World!");
```

Tudo o que você digitou no hello.js está no escopo global, posto que não foi escrito dentro de outros objetos.

O documento de referência da linguagem prescreve que, para controlar a duração da vida de todos os objetos em seus escopos, a implementação da linguagem deverá ser responsável por prover um mecanismo de gestão automatizada de memória para organizá-la de acordo com os escopos previstos no código-fonte.

A propósito, JavaScript possui várias implementações, sendo as usadas aquelas disponibilizadas pelos navegadores de Internet, já que inicialmente a linguagem se destinava apenas a automatizar procedimentos dentro do navegador Web NetScape
Navigator e, posteriormente, passou a ser adotada por todos os mais usados navegadores.  Atualmente, há também implementações para computadores Desktop (Node.JS e Deno.JS) e para dispositivos embarcados. Por ter sido criada para manipular objetos da Web, JavaScript não possui nativamente mecanismos de leitura de dados no terminal de linha de comando, ficando isso a cargo exclusivamente de bibliotecas das implementações JavaScript que são executadas neste ambinente.

A fim de aprender JavaScript sem ter a necessidade de conhecer o ambiente Web (incluindo HTML e CSS), utilizaremos aqui a implementação [NodeJS](https://nodejs.org/en) para exemplificar nossos códigos.  Esta implementação fornece a API para acessar os objetos do sistema operacional e de rede, propiciando o desenvolvimento de aplicativos servidores Web, no entanto aqui nos limitaremos ao seu uso básico com objetos do sistema.

A API Web, porém, pode ser facilmente consultada na [Mozilla Developer Network](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs).
