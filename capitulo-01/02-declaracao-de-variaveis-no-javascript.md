Para declarar uma variavel no Javascript podemos seguir uma formula simples:
`Palavra reservada + Nome da Variavel + Sinal de Atribuica + Valor da Variavel`

#### Palavras reservadas para declaracao de Variaveis no Javascript
Aqui entramos em uma boa briga, que sao as palavras reservadas para declaracao de variaveis no Javascript, temos 3 opcoes: `var, let, const`.

A palavra reservada: `var` foi a primeira forma de declaracao de variavel no Javascript, ou seja, ela eh muito mais antigas que suas irmas. Por convensao atual da linguagem, nao se deve mais declarar variaveis com com a palavra reservada `var`, pois ela esta desatualizada com relacao as outras formas de declaracao. Claro que, em codigos mais antigos com Javascript, eles estao presentes. Mas em projetos novos, nao se deve mais usa-los.

A palavra reservada: `let` eh o sucessor direto da palavra reservada `var`, as variaveis declaradas com `let` podem assumir qualquer tipo de valor, algo que falaremos depois, e o mais importante, o valor da variavel declarado com `let` pode ser alterado futuramente caso precise, o valor da variavel eh realmente variavel. Sempre que for declarado uma variavel que seu valor sera alterado futuramente, se usa a palavra reservada: `let`.

A palavra reservada: `const` declara uma constante, e nao uma variavel. O processo eh o mesmo do que a da variavel com a palavra reservada `let`, mas com um detalhe, uma vez dado um valor para uma constante, esse valor nunca mais pode ser alterado. Geralmente no Javascript, tambem por convensao da linguagem, se declara muito mais variaveis com a palavra reservada: `const` do que com a palavra reservada: `let`.