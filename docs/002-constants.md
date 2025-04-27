# Constantes e Tipos
Constantes são usadas para armazenar e representar números, caractesres ou sequências de caracteres que podem ser usados durante a execução do código, porém seus valores não podem ser alterados após a declaração.

Elas podem ser dos tipos **floatinf-point(ponto-flutuante), interger(inteiro), enumeration, character**

## Floating-point
Constantes de ponto-flutuante representam números decimais, tais como 1.2, 0.3, 10.213, 1.21, entre outros.

### Tipos de float
As constantes de ponto-flutuante podem ser divididas quanto à precisão em `float`, `double` e `long double`.

* float --> Número decimal simples, normalmente 32bits
* double --> Número decimal de precisão dupla, normalmente 64bits
* long double --> Número decimal c9223372036854775807om precisão extendida, as vees 80 ou 128 bits a depender do compilador.

### Declarando em Código
Utiliza-se `f` ou `F` para declarar um float e `l` ou `L` para declarar um long double (por padrão o `L` maiúsculo é mais usado, pois `l` pode ser confundido com o número 1).

Ex:

    float numero = 3.145f;

    double numero = 3.23823762732;

    long double numero = 3.1415926535897932384626L

## Interger
Constantes de inteiros representam números inteiros de base decimal, octal ou hexadecimal, tais como 1, 2, 8, 293, 221, -23, 32, entre outros.

Se os números tiverem o prefixo `0x` ele é considerado de base hexadecimal, caso tenha o prefixo `0` ele é considerado octal, caso o número não tenha prefixos ele é decimal.

Ex:

    Representações de 28:
    28   ---> Decimal
    0x1c ---> Hexadecimal
    034  ---> octal

### tipos de Inteiro
As constantes inteiras podem ainda ser divididas em `long`, `long long` e `unsigned` de acordo com espaço que eles ocupam na memória

* long --> 4 ou 8 bytes dependendo do sistema.
* long long --> 8 bytes independendte do sistema, permite que números maiores sejam armazenados
* unsigned --> usa apenas números positivos, dobrando o espaço para armazenamento de números maiores.

### Declarando em código
    int numero = 100;

    long numero = 1000000;

    long long numero = 9223372036854775807;

    unsigend int numero = 4000000000;


## Caractere
Constantes de caractere são formadas por um ou mais caracteres dentre os permitidos na linguagem C. Estão sempre esntre aspas simples `''`.

Quando não precedidas pela letra L, constantes de caracteres são interpretadas como inteiros, ou seja, uma constante com um único caractere possui o valor numérico do caarctere interpretado como inteiro. O valor do caractere `a`, por exemplo, é `97` em decimal e `61` em hexadecimal.

Uma constante que tenha o `L` como prefixo é do tipo `wchar_t`, representando uma cadeia longa de caracteres enquanto uma sem o prefixo possui o tipo `char` representando uma cadeia curta.


### Definindo em código
    char comum = 'x'
    wchar_t longa = L'x'


### Sequências de escape
Uma sequência de escape é representada por uma barra invertida `\` seguida de um caractere específico e pode ser utilizada, a depender do caractere depois da barra, para pular uma linha, representar uma aspa simples ou outro tipo de caractere. As sequências de escape são interpretadas pelo compilador como um caractere único.



| Sequência de escape | Representa |
|---------------------|------------|
| \a | 	Campainha (alerta)
| \b | 	Backspace
| \f | 	Avanço de formulário
| \n | 	Nova linha
| \r | 	Retorno de carro
| \t | 	Guia horizontal
| \v | 	Guia vertical
| \\' | 	Aspas simples
| \\" | 	Aspas duplas
| \\\ | 	Barra invertida
| \\? | 	Ponto de interrogação literal
| \ooo |	Caractere ASCII em notação octal
| \xhh | 	Caractere ASCII em notação hexadecimal
| \xhhhh |	Caractere Unicode em notação hexadecimal, se esta sequência de escape é usada em uma constante de caractere largo ou uma literal de cadeia de caracteres Unicode.Por exemplo, `WCHAR f = L'\x4e00'` ou `WCHAR b[] = L"The Chinese character for one is \x4e00"`.






[<- Primeiros Passos](./001-firststeps.md) ||===|| [Página inicial](../readme.md) ||===|| [Literais de cadeia ->](./003-literaisDeCadeia.md)