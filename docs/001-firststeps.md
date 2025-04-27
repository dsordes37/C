# Primeiros passos em C++
Para rodar códigos em C/C++ é preciso ter um compilador instalado, no meu caso o **g++**, compilador nativo do Ubuntu.

Após a instalação, podemos começar a codar em C++.

## Sintaxe
### Tokens
Tokens são elementos básicos reconhecidos pelo compilador, tais como **palavras chave, identificadores, constantes e operadores**. Caracters de pontuação, colchetes, chaves, parênteses e vírgulas também estão inclusos.

### Espaço em Branco
Espaços em branco são espaços vazios usados para organizar o código e garantir que ele seja interpretado da forma correta pelo compilador.

### Comentários
Comentários em C/C++ são interpretados como espaços em branco pelo compilador e servem, como em outras linguagens, para deixar mensagens, notas sobre o código e informações importantes tanto pra si quanto para outros devs que podem ler seu código no futuro.

Em C os comentários são escritos da seguinte forma:

`/* Texto do Comentário */`

### Palavras-Chave
São palavras que têm um significado específico para o compilador e por isso não podem ser usadas como identificadores.

Ex:

`if`, `for`, `inline`, `int`

### Identificadores
Identificadores são palavras usadas para dar nome a variáveis, listas, tipos, funções e etc. Identificadores **não** podem ter nomes iguais ao de alguma palavra-chave. Um identifocador é formado por um conjunto de dígitos(digits) e não dígitos(nondigits).

Dígitos:
    
    0 1 2 3 4 5 6 7 8 9

Não Dígitos:

    a b c d e f g h i j k l m n o p q r s t u v w x y z A B C D E F G H I J K L M N O P Q R S T U V W X Y Z

Um identificador **não** pode começar com um dígito

### Trígrafo
São conjuntos formados por 3 caracteres, sendo os dois primeiros símbolos de interrogação `??`, usados para representar um outro caractere único. Essa substituição ocorre durante a compilação do arquivo. 

Ex:

| Trígrafo | Caractere de Pontuação |
|----------|------------------------|
|  ??=     |  #                     |
|  ??(     |  [                     |
|  ??/     |  \                     |
|  ??)     |  ]                     |
|  ??'     |  ^                     |
|  ??<     |  {                     |
|  ??!     | \|                     |
|  ??>     |  }                     |
|  ??-     |  ~                     |



[<- Página inicial](../readme.md) ||============|| [Constantes e tipos ->](./002-constants.md)
