# UNIFOR
**nome**: Fernando gonçalves <br>
**Disciplina**: Raciocinio lógico algoritmico

## lista de exercícios 01
 
### Exercício 3
Represente , em fluxograma e pseudocódigo, um algoritmo para determinar se um número e positivo é imapar ou par.

#### Fluxograma
``` mermaid
flowchart TD
A([INICIO]) --> B{{digite um número}} 
B --> C[/num/]
C --> D{num >= 0}
D --NAO--> E{{O número deve ser positivo!}}
E --> F([FIM])
D --TRUE--> G[resto = num % 2]
G --> H{RESTO == 0}
H --FALSE--> I{{O número é impar!}}
H --TRUE--> J{{O número é par!}}
I --> F
J --> F
```
#### Pseudocódigo
```

ALGORITMO verifica_par_impar
DECLARE num, resto: INTEIRO
INICIO
ESCREVA "Digite um número:"
LEIA num
SE num > 0 ENTAO
     resto <1 num % 2
     SE resto = 0 ENTAO
          ESCREVA "O número é par!"
     SENAO
         ESCREVA "O número é impar!"
         FIM_SE
     SENAO
        ESCREVA "O NÚMERO DEVE SER POSITIVO!"
        FIM_SE
        FIM
```
#### Teste
| num | resto | num >=o | resto == 0 | Saída | 
| -- | -- | -- | -- | -- |
|-1 | false | | | "O numéro deve ser positivo" |
| 0 | true | 0 | true | "numero é par"!|
| 10 | true | 0 | true | "numero é par"!|
|11| true | 1 | falso | "numero é impar"!|




 
