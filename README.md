# OPERADORES

## + | Concatenação

Sim, o operador + é utilizado para realizar a concatenação de strings em Python. Quando você usa o operador + para unir duas strings, ele as une em uma única string, sem espaço em branco ou outro tipo de separador.
No entanto, se você tentar usar o operador + para unir uma string com um valor numérico (como uma variável inteira, por exemplo), Python não sabe como lidar com isso e retorna um erro de tipo (TypeError), indicando que não é possível concatenar um objeto do tipo "str" com um objeto do tipo "int".
Para contornar esse problema, é possível converter o valor numérico em uma string, usando a função str(), antes de concatená-lo com outra string.
Outra opção é usar a técnica de formatação de strings, que permite incluir valores numéricos em uma string de maneira mais flexível e sem a necessidade de converter os valores para strings separadamente.