# Estudo Prático de Gramáticas Formais: Derivação Sintática em C#

## Introdução e Objetivo

O objetivo desta atividade é demonstrar a aplicação prática da notação **BNF** (Backus-Naur Form) na verificação sintática da linguagem **C#**. Através da definição de um conjunto formal de regras de produção, realizaremos a **derivação passo a passo (mais à esquerda)** de uma instrução de atribuição contendo operação aritmética e operador pós-fixado:

```csharp
resultado = total * taxa++;
```

A gramática utilizada baseia-se em um recorte da especificação **ECMA-334 (C# Language Specification)**, cobrindo as regras de atribuição, precedência de operadores e pós-incremento.

---

## 1. Mapeamento de Símbolos

### Não Terminais (Variáveis Sintáticas)
* `<Statement>`
* `<ExpressionStatement>`
* `<Assignment>`
* `<PrimaryExpression>`
* `<Expression>`
* `<MultiplicativeExpression>`
* `<PostfixExpression>`
* `<Identifier>`

### Terminais (Símbolos Folha)
`resultado`, `total`, `taxa`, `=`, `*`, `++`, `;`

> *Nota:* Os identificadores `resultado`, `total` e `taxa` foram tratados diretamente como terminais para focar a análise na estrutura das expressões e operadores.

---

## 2. Recorte da Gramática BNF (C#)

```bnf
<Statement>              ::= <ExpressionStatement>

<ExpressionStatement>    ::= <Assignment> ";"

<Assignment>             ::= <PrimaryExpression> "=" <Expression>

<PrimaryExpression>      ::= <Identifier>

<Expression>             ::= <MultiplicativeExpression>

<MultiplicativeExpression> ::= <PostfixExpression> "*" <PostfixExpression>

<PostfixExpression>      ::= <Identifier>
                           | <Identifier> "++"

<Identifier>             ::= "resultado" | "total" | "taxa"
```

---

## 3. Derivação Passo a Passo (Leftmost Derivation)

A tabela abaixo descreve a substituição progressiva do não terminal mais à esquerda em cada etapa:

| Passo | Forma Sentencial Substituída | Regra Aplicada |
| :---: | :--- | :--- |
| **0** | **`<Statement>`** | *Símbolo Inicial* |
| **1** | **`<ExpressionStatement>`** | `<Statement> ::= <ExpressionStatement>` |
| **2** | **`<Assignment>`** `;` | `<ExpressionStatement> ::= <Assignment> ";"` |
| **3** | **`<PrimaryExpression>`** `=` `<Expression>` `;` | `<Assignment> ::= <PrimaryExpression> "=" <Expression>` |
| **4** | **`<Identifier>`** `=` `<Expression>` `;` | `<PrimaryExpression> ::= <Identifier>` |
| **5** | `resultado` `=` **`<Expression>`** `;` | `<Identifier> ::= "resultado"` |
| **6** | `resultado` `=` **`<MultiplicativeExpression>`** `;` | `<Expression> ::= <MultiplicativeExpression>` |
| **7** | `resultado` `=` **`<PostfixExpression>`** `*` `<PostfixExpression>` `;` | `<MultiplicativeExpression> ::= <PostfixExpression> "*" <PostfixExpression>` |
| **8** | `resultado` `=` **`<Identifier>`** `*` `<PostfixExpression>` `;` | `<PostfixExpression> ::= <Identifier>` |
| **9** | `resultado` `=` `total` `*` **`<PostfixExpression>`** `;` | `<Identifier> ::= "total"` |
| **10** | `resultado` `=` `total` `*` **`<Identifier>`** `++` `;` | `<PostfixExpression> ::= <Identifier> "++"` |
| **11** | `resultado` `=` `total` `*` `taxa` `++` `;` | `<Identifier> ::= "taxa"` |

Ao atingir o **passo 11**, a forma sentencial resulta inteiramente em símbolos terminais, validando sintaticamente a instrução C#:

```csharp
resultado = total * taxa++;
```

---

## 4. Árvore de Análise Sintática (Parse Tree)

```text
                           <Statement>
                                |
                      <ExpressionStatement>
                         /             \
                   <Assignment>        ";"
                   /    |    \
 <PrimaryExpression>   "="   <Expression>
          |                       |
     <Identifier>    <MultiplicativeExpression>
          |                /     |     \
     "resultado"   <PostfixExp> "*"  <PostfixExp>
                        |              /      \
                   <Identifier>   <Identifier> "++"
                        |              |
                     "total"        "taxa"
```

---

## 5. Análise Técnica e Conclusão

A derivação realizada exemplifica o funcionamento interno do compilador do C# (**Roslyn**):

1. **Reconhecimento da Estrutura:** Partindo do nó raiz `<Statement>`, o compilador mapeia a sequência de tokens em subestruturas sintáticas coerentes.
2. **Precedência e Operadores:** Ao diferenciar `<MultiplicativeExpression>` de `<PostfixExpression>`, a gramática garante formalmente que a ordenação e a precedência dos operadores (como a avaliação do incremento `++`) sigam as especificações da linguagem.
3. **Papel do Parser:** Enquanto este exercício realiza a derivação *top-down* (do símbolo inicial para a sentença), o *parser* do compilador efetua a análise sintática validando se a sequência de tokens fornecida pelo desenvolvedor se reduz com sucesso ao símbolo inicial.