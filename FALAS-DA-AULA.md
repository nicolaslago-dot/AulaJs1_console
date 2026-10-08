# Roteiro de falas — JavaScript: variáveis, tipos e operações

Use este roteiro como apoio durante a aula. As falas estão escritas em tom natural; adapte os exemplos e o ritmo conforme a turma.

## 1. Abertura

> Hoje vamos começar a trabalhar com JavaScript no navegador. A ideia é aprender a guardar informações, fazer alguns cálculos e conferir os resultados.
>
> Antes de começar: que informações vocês acham que um programa precisa guardar? Pode ser nome, idade, preço de um produto, pontuação de um jogo ou até uma resposta de verdadeiro ou falso.
>
> Hoje vamos aprender a representar esses dados com variáveis e constantes, conhecer alguns tipos de informação e usar operadores para fazer contas e comparações.

## 2. O que é programação client-side?

> Quando dizemos “client-side”, estamos falando de um código que é executado no dispositivo de quem está usando a página. No nosso caso, quem vai executar o JavaScript é o navegador.
>
> O HTML da página aponta para um arquivo JavaScript. O navegador carrega esse arquivo e executa as instruções. Para começar, vamos acompanhar o que o código faz pelo console.

**Ao mostrar a ligação no HTML, diga:**

> Esta linha conecta a página ao arquivo `script.js`. É nesse arquivo que vamos escrever e testar nossos primeiros comandos.

## 3. Console e `console.log()`

> O console é uma área de ferramentas do navegador que ajuda a observar o que o nosso código está fazendo. Para abrir, podemos pressionar F12 e selecionar a aba “Console”. Em alguns computadores, talvez seja preciso usar Fn junto com F12.
>
> O comando `console.log()` mostra no console o conteúdo que colocamos entre parênteses. Pode ser um texto, um número ou o resultado de uma conta.

**Demonstre e leia os resultados:**

```js
console.log("Olá, JavaScript!");
console.log(10);
console.log(5 + 3);
```

> Antes de olhar o console, o que vocês acham que vai aparecer na última linha?
>
> Isso mesmo: aparece 8, porque o JavaScript calcula a expressão antes de mostrar o resultado.

## 4. Variáveis e constantes

> Muitas vezes, um programa precisa guardar um valor para usar depois. Para isso, damos um nome a esse valor. Esse espaço com nome e valor é o que vamos usar como variável ou constante.
>
> Com `let`, criamos uma variável cujo valor pode ser atualizado. Por exemplo, a pontuação de um jogo pode começar em 10 e depois mudar para 20.

```js
let pontos = 10;
console.log(pontos);

pontos = 20;
console.log(pontos);
```

> Qual valor aparece primeiro? E qual aparece depois da alteração?
>
> Já `const` usamos quando não pretendemos reatribuir aquele valor. Por exemplo, podemos guardar o nome do jogo em uma constante.

```js
const nomeDoJogo = "Arena JS";
console.log(nomeDoJogo);
```

> Como regra prática para esta aula, comecem usando `const`. Se o valor realmente precisar mudar, usem `let`.

## 5. Tipos de dados

> Os valores que guardamos podem ser de tipos diferentes. Hoje vamos conhecer três: string, number e boolean.
>
> String é texto e fica entre aspas. Number é um número, inteiro ou decimal, sem aspas. Boolean representa uma resposta lógica: verdadeiro ou falso.

```js
const nome = "Lia";             // string
const idade = 16;               // number
const estaLogado = true;        // boolean
```

> Reparem que `true` e `false` não levam aspas. Se colocarmos aspas, o JavaScript entende que é texto, não um valor booleano.
>
> Uma dica para identificar: se está entre aspas, é texto; se é um número sem aspas, é number; se é `true` ou `false` sem aspas, é boolean.

## 6. Operadores

> Agora que sabemos guardar valores, podemos fazer operações com eles. Para as contas, temos soma com `+`, subtração com `-`, multiplicação com `*` e divisão com `/`.
>
> Também existe `%`, que retorna o resto de uma divisão. Por exemplo, 10 dividido por 3 deixa resto 1.

```js
console.log(10 + 5); // 15
console.log(10 - 5); // 5
console.log(10 * 5); // 50
console.log(10 / 5); // 2
console.log(10 % 3); // 1
```

> Além de calcular, podemos comparar. A comparação `>=` pergunta se um valor é maior ou igual a outro. O resultado será booleano: `true` ou `false`.

```js
const idade = 19;
const maiorDeIdade = idade >= 18;
console.log(maiorDeIdade);
```

> Se trocarmos a idade para 15, o que vocês esperam que apareça? A comparação continua funcionando; o resultado é que muda.

## 7. Demonstração de pequenos programas

### Nome e idade no próximo ano

> Vamos juntar algumas ideias. Guardamos um nome, uma idade e calculamos a idade do próximo ano. Primeiro, tentem prever o que vai aparecer no console.

```js
const nome = "Ravi";
let idade = 15;
const idadeNoProximoAno = idade + 1;

console.log(nome);
console.log(idadeNoProximoAno);
```

### Total de uma compra

> Agora vamos imaginar uma compra. Se cada produto custa 25 e compramos 3 unidades, multiplicamos o preço pela quantidade para encontrar o total.

```js
const preco = 25;
const quantidade = 3;
const total = preco * quantidade;

console.log(total);
```

> O mais importante é perceber o caminho: guardamos os dados, fazemos a operação e mostramos o resultado.

### Verificação com uma comparação

> Neste exemplo, a comparação verifica se a idade é pelo menos 18. Como a idade é 19, o resultado será `true`. Se usarmos 15, será `false`.

```js
const idade = 19;
const maiorDeIdade = idade >= 18;

console.log(maiorDeIdade);
```

## 8. Orientação para a prática

> Agora é a vez de vocês. Vamos editar o arquivo `js/script.js`. Depois de cada mudança, salvem o arquivo, atualizem a página e confiram o console.
>
> Se aparecer um erro, tudo bem: faz parte de programar. Leiam a mensagem, confiram as aspas, os nomes das variáveis e se o arquivo foi salvo. Chamem minha atenção se precisarem de ajuda.

### Missão 1 — Perfil

> Criem informações para um perfil: nome, idade, turma e uma informação indicando se a matrícula está ativa. Escolham o tipo adequado para cada valor e mostrem tudo com `console.log()`.

### Missão 2 — Próximo ano

> Usem a idade que vocês já criaram para calcular quantos anos a pessoa terá no próximo ano. Mostrem o resultado no console.

### Missão 3 — Compra

> Criem um preço e uma quantidade. Multipliquem os dois valores para calcular o total. Depois, mudem o preço ou a quantidade e observem como o resultado muda.

### Missão 4 — Calculadora

> Escolham dois números e mostrem a soma, a subtração, a multiplicação, a divisão e o resto da divisão.

### Desafio final

> Para o desafio final, montem uma ficha que reúna nome, idade, pontos, total de uma compra e o resultado de uma comparação. Usem pelo menos cinco comandos `console.log()` para mostrar os resultados.

## 9. Correção e revisão

> Vamos comparar algumas soluções. Pode haver nomes e valores diferentes; o importante é que o código use os tipos e as operações corretos e produza o resultado pedido.
>
> Para revisar: quando usamos `let`? E quando usamos `const`?

**Reforce os pontos principais:**

- `let` guarda um valor que pode ser reatribuído.
- `const` guarda um valor que não será reatribuído.
- String é texto; number é número; boolean é `true` ou `false`.
- Operadores fazem contas e comparações.
- `console.log()` mostra valores e resultados no console.

## 10. Encerramento

> Hoje aprendemos a ligar o JavaScript à página, acompanhar a execução pelo console, guardar dados e usar esses dados em contas e comparações.
>
> Antes de encerrarmos, pensem em uma informação que um programa poderia guardar e digam qual tipo usariam: string, number ou boolean.
>
> Na próxima aula, vamos continuar usando esses fundamentos para construir programas com mais possibilidades. Obrigado pela participação!
