# 4. Variáveis

Variáveis são identificadores de endereços de memória onde são alocados os objetos (tipos primitivos ou objetos propriamente ditos) os quais são gerenciados pela implementação da linguagem.

A sintaxe para atribuição de variáveis também chamada de instanciamento de objetos é a seguinte:

- Para variáveis globais cujo valor pode mudar ao longo do código, use:

```javascript
var identificador = valor;
```

ou

```javascript
var identificador; (o valor é undefined)
```

- Para variáveis locais cujo valor pode mudar ao longo do código, use:

```javascript
let identificador = valor;
```

ou

```javascript
let identificador; (o valor é undefined)
```

- Para definir constantes locais, use:

```javascript
const identificador = valor;
```
