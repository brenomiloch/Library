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

**Descrição:** Para resolver este problema, há duas opções. A primeira é converter a variável "Media" em uma string e, em seguida, concatená-la com a outra parte da mensagem. Isso pode ser feito usando o operador de adição (+) entre a string e a variável convertida em string:
~~~python
#CONVERTENDO EM STRING
print("A media foi de: " + str(Media))
~~~

A segunda opção é utilizar a vírgula (",") em vez de concatenar com o operador de adição. Nesse caso, a variável "Media" não precisa ser convertida em string, pois a vírgula adicionará automaticamente um espaço entre a mensagem e a variável:

~~~python
#USANDO OPERADOR ' , '
print("A media foi de: " , (Media))
~~~

&nbsp;

## %
O operador __*%*__ é chamado de operador de módulo ou resto, e ele retorna o resto da divisão entre dois números.

Por exemplo, se tivermos a __*%*__ b, o operador % retorna o resto da divisão de a por b.

O operador __*%*__ pode ser útil em diversas situações, como:

 - Verificar se um número é par ou ímpar: se um número n é divisível por 2 sem deixar resto, ou seja, se n % 2 == 0, então ele é par. Caso contrário, n é ímpar.

 - Obter a última casa decimal de um número: se tivermos um número decimal n, podemos obter a última casa decimal utilizando __n % 1__. Por exemplo, se __n = 3.14159__, então __n % 1__ retorna __*0.14159*__.

 - Calcular o dia da semana: o operador __%__ é utilizado no cálculo do dia da semana em alguns algoritmos. Por exemplo, para calcular o dia da semana de uma data, podemos utilizar a __fórmula dia_da_semana = (dia + (13*(mes+1))//5 + ano + ano//4 - ano//100 + ano//400) % 7__, onde dia, mes e ano são os componentes da data.

 - Repetir um padrão de sequência: o operador __%__ pode ser utilizado para repetir um padrão de sequência em um loop. Por exemplo, se quisermos imprimir os números de 0 a 9 em sequência infinitamente, podemos utilizar o seguinte loop: __*while True: for i in range(10): print(i, end=" ")*__, onde end=" " faz com que a função print imprima os valores separados por um espaço em vez de uma nova linha.

Essas são apenas algumas das aplicações do operador __%__. Em geral, ele é muito útil em situações que envolvem divisão e restos, e pode ser utilizado de diversas formas para resolver problemas e realizar cálculos.


&nbsp; 
&nbsp; 
&nbsp; 

# CONTROLE DE FLUXO

## if - else

A estrutura __*if*__ é usada para executar um bloco de código apenas se uma determinada condição for verdadeira. 

&nbsp;

__*🐍EXEMPLO🐍*:__
~~~python
if :
    # Codigo a ser executado se a condicao for verdadeira
~~~

O __*if*__ é seguida pela __condição__ que será avaliada. Se essa condição for verdadeira, o código abaixo do if será executado. Se a condição for falsa, o código abaixo do __*if*__ não será executado e será entrado na condição do __*else*__.


__*🐍EXEMPLO IF🐍*:__
~~~python
numero = 3

if numero > 0:
    print("O numero e positivo!")
~~~

__*🐍EXEMPLO if::else🐍*:__

A estrutura __*else*__ é usada em conjunto com o __*if*__.
 A sintaxe básica do __if - else__ é a seguinte:

~~~python
if condicao:
    # Codigo a ser executado se a condicao for verdadeira
else:
    # Codigo a ser executado se a condicao for falsa

~~~
Se a condição for verdadeira, o código dentro do __*if*__ será executado. Caso contrário, o código dentro do __*else*__ será executado.


__*❌CASO IMPAR❌*:__

~~~python
numero = 7
if numero % 2 == 0:
    print("O numero e par!")
else:
    print("O numero e impar!")
~~~

Nesse caso, a condição é numero % 2 == 0, que é __*falsa*__, pois o valor da variável numero é 7 (que é ímpar). Portanto, o código dentro do else será executado, e a mensagem "O numero e impar!" será exibida na tela.

__✅*CASO PAR*✅:__

~~~python
numero = 6
if numero % 2 == 0:
    print("O numero e par!")
else:
    print("O numero e impar!")
~~~
Nesse caso, a condição será verdadeira, pois o valor da variável numero é 6 (que é par). Portanto, o código dentro do __*if*__ será executado.


# KIVY

pip install kivy[base] kivy_examples --pre --extra-index-url https://kivy.org/downloads/simple/