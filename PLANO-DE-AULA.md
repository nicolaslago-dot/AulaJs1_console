# Aula inicial de JavaScript: Central Gamer

## Visão geral

- Público: estudantes iniciantes em desenvolvimento front-end.
- Foco: compreender o JavaScript e executar instruções simples com `console.log()`.
- Limite desta aula: os estudantes não usarão variáveis, funções próprias, eventos ou manipulação do HTML.
- HTML e CSS: já preparados pelo professor.
- Arquivo editado pelos estudantes: `js/script.js`.
- Duração total: 240 minutos, ou 4 horas.

## Objetivos

Ao final, o estudante deverá conseguir:

1. explicar o que é uma linguagem de programação;
2. diferenciar o papel de HTML, CSS e JavaScript;
3. localizar a tag que liga o JavaScript ao HTML;
4. abrir o console do navegador;
5. escrever uma instrução com `console.log()`;
6. perceber a diferença entre texto, número e conta simples no console;
7. corrigir erros básicos de aspas, parênteses e escrita do comando.

## Materiais

- editor de código;
- navegador com ferramentas de desenvolvedor;
- pasta `aula-3-javascript`;
- apresentação em `slides/Aula-JavaScript-Console-Gamer-v2.pptx`;
- arquivo do estudante em `js/script.js`;
- gabarito do professor em `js/respostas.js`.

O arquivo `respostas.js` não está ligado ao HTML. Por isso, o gabarito não aparece no console durante a atividade.

## Organização do tempo

| Parte | Tempo | Horário acumulado |
|---|---:|---:|
| Teoria | 45 min | 0 a 45 min |
| Demonstração | 45 min | 45 a 90 min |
| Atividade prática | 105 min | 90 a 195 min |
| Correção | 30 min | 195 a 225 min |
| Revisão | 15 min | 225 a 240 min |

---

## 1. Teoria: 45 minutos

### 0 a 5 min: abertura

Pergunta para a turma:

> Como podemos explicar para um computador o que ele deve fazer?

Ouça exemplos. Depois apresente a ideia de que o computador precisa de instruções claras.

### 5 a 15 min: linguagem de programação

Explique:

> Uma linguagem de programação é uma forma de escrever instruções que o computador consegue interpretar.

Use a comparação com um jogo:

- o jogador envia um comando;
- o jogo interpreta o comando;
- a tela mostra um resultado;
- um comando escrito de forma errada pode não funcionar.

Conecte a comparação à aula:

> Hoje enviaremos comandos simples ao navegador e veremos o resultado no console.

### 15 a 25 min: HTML, CSS e JavaScript

| Tecnologia | Papel simples |
|---|---|
| HTML | Organiza o conteúdo da página. |
| CSS | Cuida das cores, tamanhos e posições. |
| JavaScript | Executa instruções e cria comportamentos. |

Frase sugerida:

> O HTML monta o cenário, o CSS escolhe o visual e o JavaScript executa as ações.

Avise que, nesta primeira aula, o JavaScript ainda não modificará a página. O console será a área de treino.

### 25 a 32 min: ligação do JavaScript ao HTML

Mostre a última linha do `body`:

```html
<script src="js/script.js"></script>
```

Explique:

- `<script>` informa que a página carregará JavaScript;
- `src` indica o caminho do arquivo;
- `js/script.js` aponta para o arquivo dentro da pasta `js`;
- `</script>` fecha a tag.

### 32 a 38 min: console

Explique:

> O console é uma área do navegador que mostra mensagens, resultados e erros do JavaScript.

Como abrir:

1. pressionar `F12` ou `Fn + F12`;
2. selecionar a aba **Console**;
3. atualizar a página para executar novamente o arquivo.

### 38 a 45 min: primeira instrução

```js
console.log("Jogador conectado!");
```

Explique cada parte:

| Parte | Explicação simples |
|---|---|
| `console` | A ferramenta do navegador que usaremos. |
| `.` | Liga a ferramenta à ação. |
| `log` | A ação de registrar ou mostrar algo. |
| `( )` | Guardam o conteúdo enviado. |
| `" "` | Indicam um texto. |
| `;` | Marca o fim da instrução. |

Frase para a turma:

> `console.log()` significa: “console, mostre este conteúdo”.

---

## 2. Demonstração: 45 minutos

### 45 a 55 min: arquivos do projeto

1. Abra a pasta `aula-3-javascript`.
2. Mostre `index.html`, `css/estilos.css` e `js/script.js`.
3. Reforce que os estudantes editarão apenas o JavaScript.
4. Localize a tag `<script>` no fim do HTML.

### 55 a 65 min: primeiro resultado

1. Abra `index.html` no navegador.
2. Abra o console.
3. Localize `=== CENTRAL GAMER ===` e `Jogador conectado!`.
4. Relacione cada resultado à linha correspondente no arquivo.

Pergunte:

- Em qual arquivo está o comando?
- Onde apareceu o resultado?
- A mensagem apareceu dentro da página?

### 65 a 75 min: ciclo de teste

Troque uma mensagem:

```js
console.log("Minha primeira fase com JavaScript!");
```

Mostre o ciclo:

1. editar;
2. salvar;
3. voltar ao navegador;
4. atualizar;
5. observar o console.

### 75 a 82 min: ordem das instruções

```js
console.log("Primeira mensagem");
console.log("Segunda mensagem");
console.log("Terceira mensagem");
```

Peça que a turma preveja a ordem. Depois execute e confirme que o navegador lê de cima para baixo.

### 82 a 90 min: texto, número e conta

```js
console.log("100");
console.log(100);
console.log("50 + 25");
console.log(50 + 25);
```

Explique:

- com aspas, o conteúdo é texto;
- sem aspas, `50 + 25` é calculado;
- tipos serão estudados com mais detalhes em outra aula.

---

## 3. Atividade prática: 105 minutos

Os estudantes editam somente `js/script.js`.

### 90 a 100 min: preparação

1. Confirme que todos abriram o arquivo correto.
2. Peça que abram o console.
3. Oriente a salvar e atualizar a página após cada alteração.
4. Faça cada estudante mudar `Jogador conectado!` para confirmar o fluxo.

### 100 a 125 min: missão 1, perfil do jogador

Cada estudante deve mostrar:

1. nome;
2. turma;
3. jogo, esporte, música ou série de que gosta.

Critérios:

- uma instrução por linha;
- textos entre aspas;
- nenhum erro vermelho no console.

### 125 a 155 min: missão 2, pontos

Tarefas:

1. mostrar o número `100` sem aspas;
2. mostrar o resultado de `50 + 25`;
3. mostrar `"50 + 25"` e depois `50 + 25`;
4. explicar por que os dois últimos resultados são diferentes.

### 155 a 190 min: missão 3, ficha gamer

Crie cinco linhas:

```text
=== FICHA GAMER ===
Nome: ...
Turma: ...
Hobby favorito: ...
=== FIM DA FICHA ===
```

Cada linha deve vir de um `console.log()` diferente.

### 190 a 195 min: chefe final

Crie uma tela de vitória com pelo menos cinco linhas. Ela precisa ter:

- uma mensagem de vitória;
- um número sem aspas;
- o resultado de uma conta simples;
- uma mensagem final.

---

## 4. Correção: 30 minutos

### 195 a 205 min: correção coletiva

Abra `js/respostas.js` apenas no editor. Compare as respostas com as soluções da turma.

Aceite textos pessoais diferentes quando o estudante tiver usado corretamente `console.log()`.

### 205 a 215 min: erros comuns

Texto sem aspas:

```js
console.log(Jogador conectado!);
```

Correção:

```js
console.log("Jogador conectado!");
```

Parêntese não fechado:

```js
console.log("Jogador conectado!";
```

Correção:

```js
console.log("Jogador conectado!");
```

Letra maiúscula no comando:

```js
Console.log("Olá!");
```

Correção:

```js
console.log("Olá!");
```

### 215 a 225 min: leitura de erros

Oriente a turma a:

1. ler a primeira mensagem vermelha;
2. observar o arquivo e o número da linha;
3. conferir aspas, parênteses e a escrita de `console.log`;
4. corrigir uma coisa por vez;
5. salvar e atualizar.

---

## 5. Revisão: 15 minutos

### 225 a 235 min: perguntas rápidas

1. O que é uma linguagem de programação?
2. Qual é o papel do HTML?
3. Qual é o papel do CSS?
4. Qual é o papel do JavaScript?
5. Para que serve a tag `<script>`?
6. O que é o console?
7. O que faz `console.log()`?
8. Por que um texto usa aspas?
9. Qual é o resultado de `console.log(4 + 3);`?
10. Qual é o resultado de `console.log("4 + 3");`?

### 235 a 240 min: bilhete de saída

Peça três respostas curtas:

1. Hoje eu aprendi que...
2. Eu consegui executar...
3. Minha dúvida ainda é...

## Avaliação simples

| Critério | Conseguiu | Precisa de apoio |
|---|---|---|
| Abriu o console |  |  |
| Encontrou a mensagem inicial |  |  |
| Alterou uma mensagem e viu o novo resultado |  |  |
| Usou aspas em textos |  |  |
| Mostrou um número sem aspas |  |  |
| Mostrou o resultado de uma conta |  |  |
| Criou a ficha gamer |  |  |
| Explicou o uso de `console.log()` |  |  |

## Próxima aula sugerida

Variáveis com `let` e `const`, mantendo o console como saída. Assim, a turma avança sem misturar muitos conceitos.
