# 1. Características da linguagem: código-fonte, escopo, gestão de memória e implementações

JavaScript é uma linguagem de programação que suporta aos paradigmas sequencial, estruturado, procedural, funcional e orientado a objetos.  O código fonte JavaScript deve
ser inserido em um arquivo de texto de sistema operacional com extensão .js, ou seja, um programa nomeado hello teria seu código-fonte em um arquivo nomeado hello.js.
Ademais, o código-fonte é dividido em dois trechos: trecho de escopo global e trecho de escopo local. O trecho de escopo global manipula os objetos da linguagem que
serão armazenados em memória durante todo o tempo de execução do programa ao passo que o trecho de escopo local contém objetos que durarão apenas enquanto este trecho de
código estiver sendo executado.

A gestão de memória é automatizada pela implementação da linguagem a qual é responsável por organizá-la de acordo com os escopos previstos no código-fonte.
A respeito das várias implementações de JavaScript, vale notar que inicialmente a linguagem se destinava apenas a automatizar procedimentos dentro do navegador Web NetScape
Navigator, sendo, posteriormente, adotada por todos os mais usados navegadores.  Atualmente, há também implementações para computadores Desktop (Node.JS e Deno.JS) e
para dispositivos embarcados.

A fim de aprender JavaScript sem ter a necessidade de conhecer o ambiente Web (incluindo HTML e CSS), utilizaremos aqui a implementação [NodeJS](https://nodejs.org/en)
para exemplificar nossos códigos.  
