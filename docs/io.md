# 5. Operações de entrada e saída de dados

Para realizar saída de dados na tela, use:

```javascript
let x = 2;
console.log(x);
```

Para realizar leitura de dados do teclado, use:

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
