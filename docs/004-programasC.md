# Programas em C
Um programa de origem C é uma coleção de políticas, pragmas, declarações, definições, funções e regras divididas em um ou mais arquivos de origem ou unidades de tradução, que é como chamamos a entrada que damos ao compilador.


Esses arquivos de origem não precisam ter instruções executáveis. Podemos ter arquivos só com variáveis ou constantes que são acessadas por outros arquivos, tornando o código mais organizado e facilitanto a manutenção.

# Diretivas para o pré-processador
Uma política ou diretiva para pré-processador realiza ações específicas no texto do programa antes da compilação, como substituir toda ocorrência de um trecho de código por outro

Ex:

    #define MAX 100

substitui todas as ocorrências de `MAX` pelo número `100`.


| Diretivas | Função |
|-----------|--------|
| #include | Insere conteúdo de um arquivo no ponto onde a diretiva foi usada |
| #if, #ifdef, #ifndef, #else, #elif, #endif | Controla a compilação condicional. |
| #pragma | Fornece instruções específicas ao compilador, como inclusão de arquivos de cabeçalho e alinhamento de espaços na memória.  |
| #error | Gera um erro na compilação com uma mensagem personalisada |
| #warning | Exibe um aviso durante a compilação |
| #line | altera o número de linha e possivelmente o nome do arquivo ao ser executado. |



[<- Literais de cadeia](./003-literaisDeCadeia.md)||===|| [Página inicial](../readme.md)||===||[Declarações ->](./005-declarations.md)