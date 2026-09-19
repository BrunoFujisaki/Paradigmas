# 🌙 Linguagem de Programação Lua

---

## 💡 Paradigmas da Linguagem

Lua é normalmente descrita como uma **linguagem multiparadigma**. Em vez de fornecer uma especificação complexa e rígida para se ajustar a um único modelo, Lua oferece um pequeno conjunto de características gerais que podem ser estendidas para resolver diferentes tipos de problemas.

### Destaques de Design e Funcionalidades:
* **Orientação a Objetos Flexível:** Lua não possui suporte explícito nativo à herança ou classes, mas permite implementá-las com facilidade utilizando **`metatables`**.
* **Programação Funcional:** Permite utilizar técnicas avançadas de programação funcional, contando com suporte a **escopos lexicais completos** e funções de primeira classe.
* **Tipos de Dados Simples e Eficientes:** Suporta nativamente um pequeno número de estruturas estruturais básicas:
  * Dados atômicos
  * Valores booleanos
  * Números (*dupla precisão em ponto flutuante por padrão*)
  * Strings
* **Estrutura de Dados Unificada:** Estruturas comuns como matrizes, conjuntos, listas e registros são todas representadas através de **tabelas (`tables`)**, a principal estrutura de dados da linguagem.

---

## 💻 Exemplos de Código

Abaixo está um exemplo básico em Lua demonstrando a exibição de uma mensagem inicial e o cálculo da tabuada a partir de um valor digitado pelo usuário.

```lua
-- Exibição de mensagem inicial
print("Olá, mundo!\n")

-- Leitura e conversão da entrada do usuário
print("Digite um número:")
local n = tonumber(io.read())

-- Laço para cálculo e exibição da tabuada
for i = 1, 10 do
    print(n .. " x " .. i .. " = " .. (n * i))
end
```

---

## 💼 Oportunidades de Trabalho e Faixas Salariais

Confira algumas vagas focadas em desenvolvimento Lua com remuneração em dólar:

| Posição / Empresa | Plataforma | Faixa Salarial | Link |
| :--- | :--- | :--- | :--- |
| **Senior Lua Developer (Roblox – AI Code Evaluation)** | Upwork / LinkedIn | **US$ 50,00 – US$ 65,00** / hora | [Ver Vaga](https://br.linkedin.com/jobs/view/copy-of-senior-lua-developer-roblox-%E2%80%93-ai-code-evaluation-at-upwork-4443268669) |
| **Lua Programmer** | Alignerr / LinkedIn | **Até US$ 60,00** / hora *(conforme disponibilidade)* | [Ver Vaga](https://br.linkedin.com/jobs/view/lua-programmer-at-alignerr-4447234822) |
