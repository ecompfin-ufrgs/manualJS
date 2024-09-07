# 3. Objetos e tipos de dados em JavaScript

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
