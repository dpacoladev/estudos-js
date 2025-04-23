Para declarar uma variável no JavaScript, podemos seguir uma fórmula simples:

`Palavra reservada + Nome da variável + Sinal de atribuição + Valor da variável`

### Palavras reservadas para declaração de variáveis no JavaScript

No mundo das linguagens de programação, existe algo que eu não compreendo. Existem varias formas de fazer exatamente a mesma coisa. Seria muito mais simples ter somente uma. Mas como nem tudo na vida são flores, no JavaScript existem mais que uma forma de declarar uma simples variável. Aqui entramos em uma boa discussão: quais são as palavras reservadas para a declaração de variáveis no JavaScript? Temos três opções: `var`, `let` e `const`.

#### `var`
A palavra reservada `var` foi a primeira forma de declarar variáveis no JavaScript, ou seja, é muito mais antiga que suas "irmãs". Pela convenção atual da linguagem, **não se deve mais declarar variáveis usando `var`**, pois ela está desatualizada em relação às outras formas de declaração. Claro, em códigos JavaScript mais antigos, você ainda encontrará `var` com frequência, mas em **projetos modernos, seu uso não é recomendado**.

```
var nome = "Dalton"
var idade = 23
var altura = 1.8

nome = "Diego"
idade = 35
altura = 1.9
```

#### `let`
A palavra reservada `let` é o **sucessor direto de `var`**. As variáveis declaradas com `let` podem assumir qualquer tipo de valor (como veremos mais adiante) e, o mais importante: **o valor da variável pode ser alterado futuramente**, caso necessário. Ou seja, o valor é realmente "variável". Sempre que for declarar uma variável cujo valor será modificado, deve-se usar a palavra reservada `let`.

```
let nome = "Dalton"
let idade = 23
let altura = 1.8

nome = "Diego"
idade = 35
altura = 1.9
```

#### `const`
A palavra reservada `const` declara uma **constante**, e não exatamente uma variável. O processo de declaração é semelhante ao de `let`, mas com uma diferença fundamental: **uma vez atribuído um valor à constante, esse valor não pode mais ser alterado**. Por convenção, no JavaScript moderno, declara-se **muito mais variáveis usando `const` do que `let`**, justamente para garantir mais segurança e previsibilidade no código.]

```
const nome = "Dalton"
const idade = 23
const altura = 1.8

nome = "Diego" // |
idade = 35     // | ❌ Errado! Nao se pode alterar uma constante.
altura = 1.9   // |
```

### Nome de Variáveis no JavaScript

Bom, o nome de uma variável em JavaScript é o que vem logo após a palavra reservada de declaração. Todo e qualquer caractere **pode ser utilizado**, mas existem algumas **convenções** e **peculiaridades importantes** sobre nomes de variáveis. Vamos a elas:

#### `Não conter espaço`
O nome de uma variável **não pode conter espaços**, pois, se houver, o interpretador JavaScript **não conseguirá entender** onde começa e onde termina o nome da variável.

```
let nome completo = "Dalton Pacola Franco" // ❌ Errado
let nomeCompleto = "Dalton Pacola Franco"  // ✅ Correto
```

#### `Caracteres proibidos como primeiro caractere`
Existem caracteres que **não podem ser o primeiro** em um nome de variável, como:

- **Números** (`0` a `9`)
- **Símbolos especiais** como `@`, `#`, `-`, `+`  
    **Exceção**: os símbolos `_` (underline) e `$` (cifrão) **são permitidos** como primeiro caractere.

```
let nomeCompleto = "Dalton Pacola Franco" // ✅ Correto
let 1nome = "Dalton Pacola Franco"        // ❌ Errado
let @rrombado = "Alexandre..."            // ❌ Errado
let #jogoDaVelha = true                   // ❌ Errado
let +OuMenos = false                      // ❌ Errado
let -OuMais = true                        // ❌ Errado
let maiorQue18Anos = true                 // ✅ Correto
let $reais = 15                           // ✅ Correto
let _variavelPrivada = 1.7                // ✅ Correto
```

#### `camelCase`
Por **convenção**, os nomes de variáveis em JavaScript são escritos no formato `camelCase`. Isso significa:

- A **primeira letra** do nome da variável deve ser **minúscula**
- Se o nome tiver mais de uma palavra, a **primeira letra de cada palavra seguinte** deve ser **maiúscula**

Embora o JavaScript permita outras formas, **seguir essa convenção deixa o código mais legível e padronizado**.

```
let nomeCompleto = "Dalton Pacola Franco"  // ✅ Correto
let Nomecompleto = "Dalton Pacola Franco"  // ⚠️ Fora de convenção
let nomecompleto = "Dalton Pacola Franco"  // ⚠️ Fora de convenção
let NomeCompleto = "Dalton Pacola Franco"  // ⚠️ Fora de convenção
let nome_completo = "Dalton Pacola Franco" // ⚠️ Fora de convenção
```


### Sinal de Atribuição no JavaScript

Depois do nome da variável, vem o sinal de atribuição de valor. O sinal de atribuição no JavaScript é o mesmo utilizado em diversas outras linguagens: o sinal de igual `=`.  No entanto, **ele não deve ser lido como "igual" na programação**, e sim como **"atribuição"**.  Mais adiante, veremos que a comparação de igualdade é feita com outros sinais no JavaScript.

Portanto, ao observar a seguinte declaração de variável:

```
let nomeCompleto = "Dalton Pacola Franco"
```
Devemos interpretar da seguinte forma:  
Na variável `nomeCompleto` está sendo **atribuído o valor** `"Dalton Pacola Franco"`.


### Valor da Variável

Depois do sinal de atribuição, vem o **valor** que a variável irá armazenar.  
Esse valor pode ser um **texto** (_String_), **número** (_Number_), **decisão binária** (_Boolean_) ou até mesmo um **objeto** (_Object_). Veremos mais adiante os tipos de dados com mais detalhes. E sim, mesmo o JavaScript sendo **fracamente tipado**, ele possui tipos de dados definidos.

Abaixo, alguns exemplos de valores atribuídos a variáveis:
```
let nomeCompleto = "Dalton Pacola Franco"  // String (Texto)
let idade = 22                             // Number (Número)
let altura = 1.8                           // Number (Número)
let possui18Anos = true                    // Boolean (Verdadeiro)
let temCarro = false                       // Boolean (Falso)

let usuario = {                            // |
	nomeCompleto: "Dalton Pacola Franco",  // |
	idade: 22,                             // |
	altura: = 1.8,                         // | - Object (Objeto)
	possui18Anos: = true,                  // |
	temCarro: = false                      // |
}                                          // |
``` 


Para este primeiro momento, podemos perceber que **cada variável possui um nome e um único valor atribuído a ela**. Mais adiante, veremos formas de **atribuir múltiplos valores a uma mesma variável** (inclusive, já mostramos um exemplo com o uso de objetos).

Além disso, surgem outras questões interessantes que também serão abordadas futuramente, como:

- O que acontece **se eu não atribuir um valor a uma variável**?
- Onde, de fato, o **valor da variável é armazenado**?
- Existe uma forma de **converter um tipo de valor em outro**?

Essas dúvidas são comuns no início, e todas serão respondidas ao longo das anotacoes!