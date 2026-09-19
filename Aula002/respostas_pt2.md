# Exercícios sobre Linguagens de Programação

---

### **15. A primeira aplicação de Java não foi a Web, mas a Web impulsionou sua adoção. Explique como mudanças de contexto podem reposicionar uma linguagem.**

> **Resposta:**
> 
> Na década de 1990, o **Java** foi originalmente criado como uma linguagem confiável voltada para sistemas embarcados e eletrônicos de consumo. Contudo, seus primeiros produtos comerciais nessa área não obtiveram sucesso no mercado. 
> 
> Com a rápida popularização da Web a partir de 1993, a linguagem ganhou enorme destaque por se mostrar extremamente útil para o desenvolvimento na Internet — principalmente devido aos *applets* (pequenos programas executados diretamente nos navegadores). 
> 
> Assim, nos primeiros anos de sua popularização, a Web tornou-se sua principal aplicação, impulsionando o Java de uma linguagem pouco utilizada para uma das tecnologias mais presentes e essenciais do dia a dia da computação.

---

### **16. Compare Perl, JavaScript, PHP, Python, Ruby e Lua usando três eixos: domínio inicial, estruturas de dados e estratégia de implementação. Evite concluir que todas são iguais por serem chamadas de scripting.**

> **Resposta:**

| Linguagem | Domínio Inicial | Estruturas de Dados Primárias | Estratégia de Implementação |
| :--- | :--- | :--- | :--- |
| **Perl** | Processamento de texto e administração de sistemas | Escalares, vetores e *hashes* | Compilada para representação intermediária |
| **JavaScript** | Programação no navegador (*client-side*) | Strings, vetores e objetos baseados em protótipos | Tradicionalmente interpretada pelo navegador |
| **PHP** | Ferramenta para páginas Web estáticas/dinâmicas | Combinação de vetores e *hashes* | Interpretada no servidor (*server-side*) |
| **Python** | Administração de sistemas e automação | Listas, tuplas e dicionários | Tipagem dinâmica, OO e coleta de lixo (*Garbage Collection*) |
| **Ruby** | Propósito geral e Orientação a Objetos | Tudo é objeto; métodos podem ser adicionados dinamicamente | Interpretada/Compilada via máquina virtual (*bytecode*) |
| **Lua** | *Scripting* genérico e extensibilidade | Estrutura unificada baseada em **tabelas** | Traduzida para código intermediário antes da interpretação |

---

### **17. C# foi apresentada como evolução no ambiente .NET. Compare duas decisões de C# com suas correspondentes em Java ou C++ e explique o problema que pretendem resolver.**

> **Resposta:**
> 
> Lançado pela Microsoft em 2000 como a linguagem principal da plataforma .NET, o **C#** inspirou-se em C++ e Java, introduzindo melhorias para focar em segurança, simplicidade e expressividade.
> 
> 1. **Delegates (*Delegados*)**:
>    * **Problema/Substituição:** Substituem os ponteiros para funções do C++ (que são inseguros) e evitam a proliferação de interfaces verbosas/complexas do Java.
>    * **Solução:** São referências seguras e orientadas a objetos para subprogramas. Facilitam o tratamento de *callbacks*, eventos e execução de *threads*, unindo flexibilidade e segurança de tipos.
>
> 2. **Boxing e Unboxing**:
>    * **Problema/Substituição:** Resolve a separação rígida entre tipos primitivos e objetos sem a necessidade de criação manual de classes *wrapper*.
>    * **Solução:** Unifica o sistema de tipos fazendo com que todos os tipos derivem de `System.Object`. Permite converter valores primitivos diretamente em objetos (*boxing*) e recuperá-los (*unboxing*), simplificando a manipulação em coleções genéricas.

---

### **18. Diferencie XSLT e JSP quanto a entrada, processamento e saída. Por que ambas podem ser chamadas de linguagens híbridas de marcação e programação?**

> **Resposta:**

#### **Diferenças Principais**

* **XSLT**
  * **Entrada:** Documento XML.
  * **Processamento:** Aplica regras de transformação, ordenação e filtragem orientadas a padrões (*pattern matching*).
  * **Saída:** Novo documento estruturado (XML, HTML ou texto puro).

* **JSP (com JSTL/JS)**
  * **Entrada:** Requisições HTTP e parâmetros de contexto.
  * **Processamento:** Executa lógica no lado do servidor por meio de *tags* estruturadas e rotinas Java.
  * **Saída:** HTML dinâmico gerado para exibição no navegador do cliente.

#### **Por que são consideradas Linguagens Híbridas?**
Ambas incorporam **recursos clássicos de programação** (como estruturas condicionais, laços de repetição e manipulação de dados) em meio à sintaxe de **linguagens de marcação** (baseadas em *tags*), que originalmente serviam apenas para a apresentação ou estruturação passiva de informações.

---

### **19. Crie uma linha do tempo com oito linguagens de pelo menos quatro paradigmas. Para cada ligação, escreva o tipo de influência; não use apenas setas cronológicas.**

> **Resposta:**

* **1957 — Fortran** *(Paradigma Imperativo)*
  * *Influência:* Estabeleceu a base da programação imperativa, introduzindo expressões matemáticas traduzíveis e laços de repetição.
* **1958 — Lisp** *(Paradigma Funcional)*
  * *Influência:* Pioneira no paradigma funcional, introduzindo o processamento baseado em listas, expressões condicionais de primeira classe e recursão.
* **1960 — ALGOL 60** *(Paradigma Imperativo/Estruturado)*
  * *Influência:* Sintetizou conceitos do Fortran adicionando blocos de código, escopo local e ortogonalidade, servindo de modelo gramatical para quase todas as linguagens imperativas posteriores.
* **1967 — Simula 67** *(Paradigma Orientado a Objetos)*
  * *Influência:* Evoluiu do ALGOL 60 ao introduzir os conceitos fundamentais de classes, objetos e herança.
* **1972 — Prolog** *(Paradigma Lógico/Declarativo)*
  * *Influência:* Inovou ao introduzir a programação lógica baseada em fatos, regras e motores de inferência.
* **1983 — C++** *(Paradigma Multi-paradigma / OO + Imperativo)*
  * *Influência:* Combinou o desempenho e controle de baixo nível da linguagem C com o modelo de orientação a objetos herdado do Simula 67.
* **1995 — Java** *(Paradigma Orientado a Objetos)*
  * *Influência:* Refinou as ideias de C++, eliminando a manipulação direta de ponteiros e adotando uma máquina virtual com *Garbage Collector* e verificação de limites em tempo de execução para garantir maior segurança.
* **2000 — C#** *(Paradigma Multi-paradigma)*
  * *Influência:* Surgiu no ecossistema .NET absorvendo e refinando a sintaxe e modelo de execução do Java, integrando novos recursos de linguagem como *structs*, *delegates* e propriedades nativas.

---

### **20. Estudo de caso: uma equipe precisa escolher tecnologias para cálculo científico, regras declarativas, aplicação Web interativa e firmware restrito. Proponha famílias de linguagens, justifique historicamente cada escolha e explicite dois trade-offs.**

> **Resposta:**

#### **1. Escolha de Tecnologias e Justificativa Histórica**

* **Cálculo Científico $\rightarrow$ Fortran**
  * *Justificativa:* Historicamente projetado e continuamente otimizado para operações matemáticas intensivas e vetoriais, oferecendo altíssimo desempenho com tipos e alocação de memória estáticos.
* **Regras Declarativas $\rightarrow$ Prolog**
  * *Justificativa:* Criado especificamente para resolução de problemas de inteligência artificial e lógica, permitindo expressar o conhecimento por meio de fatos e regras onde a execução é resolvida pelo sistema de inferência.
* **Aplicação Web Interativa $\rightarrow$ JavaScript / PHP**
  * *Justificativa:* O **JavaScript** consolidou-se como o padrão universal *client-side* para interatividade no navegador, enquanto o **PHP** evoluiu historicamente como uma solução simples e robusta para renderização e lógica no servidor (*server-side*).
* **Firmware Restrito $\rightarrow$ C / C++**
  * *Justificativa:* Desenvolvidas com proximidade direta ao hardware, permitem controle preciso de memória, compilação para código de máquina altamente eficiente e footprint mínimo de execução.

#### **2. Trade-offs Principais**

1. **Confiabilidade $\times$ Eficiência:**
   * Linguagens como Java e C# oferecem maior segurança de memória através do *Garbage Collector* e checagens em tempo de execução, mas cobram um custo computacional adicional. Por outro lado, linguagens como C e C++ priorizam a velocidade máxima de execução sacrificando a segurança automática de memória.
2. **Legibilidade / Expressividade $\times$ Facilidade de Escrita:**
   * Linguagens de alto nível e dinâmicas permitem construir funcionalidades rapidamente com poucas linhas de código, facilitando o desenvolvimento inicial. Em contrapartida, essa maior flexibilidade pode comprometer a legibilidade, a checagem de tipos em tempo de compilação e a manutenção em sistemas de grande porte.