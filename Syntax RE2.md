# Sintaxe

Expressões regulares são notações para descrever conjuntos de cadeias de caracteres. Quando uma determinada string está no conjunto descrito por uma expressão regular, costumamos dizer que a expressão regular corresponde à string.

A expressão regular mais simples é um único caractere literal. Exceto para os metacaracteres como `*+?()|`, os caracteres correspondem a si mesmos. Para corresponder a um metacaractere, faça um escape com uma barra invertida: `\+` corresponde a um caractere literal de mais.

Duas expressões regulares podem ser alternadas ou concatenadas para formar uma nova expressão regular: se _e1_ corresponde a _s_ e e2 corresponde a _t_, então _e1_ | _e2_ corresponde a _s_ ou _t_,  e _e1e2_ corresponde a _st_.

Os metacaracteres `*`, `+` e `?` são operadores de repetição:
* e1`*` corresponde a uma sequência de zero ou mais strings (possivelmente diferentes), cada uma correspondendo a e1;
* e1`+` corresponde a um ou mais; 
* e1`?` corresponde a zero ou um.




# Referencias:

Syntax - https://github.com/google/re2/wiki/Syntax
