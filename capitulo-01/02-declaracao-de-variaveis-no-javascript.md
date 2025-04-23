Para declarar uma variável no JavaScript, podemos seguir uma fórmula simples:

`Palavra reservada + Nome da variável + Sinal de atribuição + Valor da variável
`
### Palavras reservadas para declaração de variáveis no JavaScript

Aqui entramos em uma boa discussão: quais são as palavras reservadas para a declaração de variáveis no JavaScript? Temos três opções: `var`, `let` e `const`.

#### `var`
A palavra reservada `var` foi a primeira forma de declarar variáveis no JavaScript, ou seja, é muito mais antiga que suas "irmãs". Pela convenção atual da linguagem, **não se deve mais declarar variáveis usando `var`**, pois ela está desatualizada em relação às outras formas de declaração. Claro, em códigos JavaScript mais antigos, você ainda encontrará `var` com frequência, mas em **projetos modernos, seu uso não é recomendado**.

#### `let`
A palavra reservada `let` é o **sucessor direto de `var`**. As variáveis declaradas com `let` podem assumir qualquer tipo de valor (como veremos mais adiante) e, o mais importante: **o valor da variável pode ser alterado futuramente**, caso necessário. Ou seja, o valor é realmente "variável". Sempre que for declarar uma variável cujo valor será modificado, deve-se usar a palavra reservada `let`.

#### `const`
A palavra reservada `const` declara uma **constante**, e não exatamente uma variável. O processo de declaração é semelhante ao de `let`, mas com uma diferença fundamental: **uma vez atribuído um valor à constante, esse valor não pode mais ser alterado**. Por convenção, no JavaScript moderno, declara-se **muito mais variáveis usando `const` do que `let`**, justamente para garantir mais segurança e previsibilidade no código.