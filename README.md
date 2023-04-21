# OPERADORES

## ➕
Operador **➕** é utilizado para realizar a concatenação de __*strings*__ em __*PYTHON*__. Quando você usa o operador **➕** para unir duas __*strings*__, ele as une em uma única __*strings*__, sem espaço em branco ou outro tipo de separador. No entanto, se você tentar usar o operador **➕** para unir uma string com um valor numérico (como uma variável __*inteira(int)*__ ou __*string(str)*__ , por exemplo), __*PYTHON*__ não sabe como lidar com isso e retorna um erro de tipo (__*TypeError*__), indicando que não é possível concatenar um objeto do tipo __*"str"*__ 
com um objeto do tipo __*"int"*__.
Para contornar esse problema, é possível converter o valor numérico em uma __*string*__, usando a função __*str()*__, antes de concatená-lo com outra __*string*__. Outra opção é usar a técnica de formatação de __*strings*__, que permite incluir valores numéricos em uma __*string*__ de maneira mais flexível e sem a necessidade de converter os valores para __*strings*__ separadamente.

__*🐍EXEMPLO DE CASO🐍*__
~~~python
Nota_1 = int(input("Digite a primeira nota bimestral: "))
Nota_2 = int(input("Digite a segunda nota bimestral: "))
Media = Nota_1 + Nota_2
print("A media foi de: " + (Media))
~~~
__*❌ERRADO:❌*__

**Descrição:** No código abaixo a __*print*__ está concatenando uma string com um valor numérico inteiro, ao rodar o código assim, dará erro:
~~~python
print("A media foi de: " + (Media))
~~~ 

__*✅EXEMPLO CERTO:✅*__

**Descrição:** Para resolver esse problema, temos duas opções, primeira converter a variavel Media em string e depois concatela a string ou a segunda é utilizar a vírgula __* , *__ em vez de concatená-la com o operador __* + *__

~~~python
#CONVERTENDO EM STRING
print("A media foi de: " + str(Media))
~~~
~~~Python
#USANDO OPERADOR ' , '
print("A media foi de: " , (Media))
~~~~
