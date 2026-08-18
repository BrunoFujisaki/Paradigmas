# História das Linguagens de Programação

## 1. A genealogia das linguagens não é uma escada de progresso

A afirmação de que a genealogia das linguagens de programação não é uma escada de progresso significa que a evolução das linguagens não ocorre em uma linha reta, na qual uma tecnologia mais nova é sempre superior e substitui completamente a anterior. Pelo contrário, conceitos antigos e novos coexistem de acordo com as necessidades práticas.

Dois fatores históricos que fazem uma linguagem influenciar outra sem necessariamente substituí-la são:

1. **Inovação conceitual e teórica:** uma linguagem pode introduzir novos paradigmas, formalismos ou estruturas que servem como "DNA" ou base conceitual para o projeto de tecnologias futuras, mesmo que a linguagem pioneira em si perca espaço ou fracasse comercialmente. Um exemplo é o forte legado estrutural e formal do **ALGOL 60** sobre as linguagens imperativas subsequentes.

2. **Interoperabilidade e integração em ecossistemas comuns:** o desenvolvimento de novas plataformas e frameworks unificados, como o ecossistema **.NET**, permite que linguagens de paradigmas diferentes influenciem e colaborem entre si no desenvolvimento baseado em componentes. Elas podem compartilhar o mesmo sistema de tipos e código intermediário sem que uma precise eliminar a outra.

---

## 2. Plankalkül e sua importância histórica

A **Plankalkül** é relevante porque foi uma das primeiras propostas de uma linguagem de programação de alto nível. Mesmo sem ter sido implementada em sua época, seu projeto antecipou conceitos fundamentais que só apareceriam em outras linguagens muitos anos depois.

Entre os recursos antecipados por seu projeto estão:

* Estruturas de dados;
* Tipos de dados;
* Operações sobre dados estruturados;
* Uso de variáveis e atribuições;
* Conceitos relacionados a programação de alto nível.

Um dos principais valores desses recursos foi mostrar que a programação poderia ser estruturada em conceitos mais abstratos do que simples instruções de máquina. Isso ajudou a estabelecer ideias que posteriormente seriam fundamentais para o desenvolvimento das linguagens de programação modernas.

---

## 3. Short Code, Speedcoding e A-0/A-1/A-2

### Problema enfrentado

Os primeiros programadores enfrentavam extrema dificuldade, lentidão e alta taxa de erros ao programar os primeiros computadores diretamente em código de máquina, utilizando instruções numéricas e endereços absolutos.

### Estratégias adotadas

* **Short Code:** utilizava uma estratégia de **interpretação**, funcionando como uma espécie de simulador de uma máquina virtual, facilitando a programação em relação ao código de máquina.
* **Speedcoding:** também adotava uma estratégia baseada em **interpretação**, oferecendo uma forma mais simples de programar operações, especialmente cálculos numéricos e de ponto flutuante.
* **A-0, A-1 e A-2:** utilizavam uma estratégia baseada na **expansão de pseudocódigos em subprogramas de código de máquina**, funcionando de maneira semelhante a macros em linguagem de montagem.

### Por que não são simplesmente compiladores modernos?

Chamá-los simplesmente de compiladores modernos seria impreciso porque eles não realizavam o processo completo de compilação que conhecemos atualmente, envolvendo etapas como:

* análise léxica;
* análise sintática;
* análise semântica;
* geração de código;
* otimização do código.

O **Short Code** e o **Speedcoding** eram essencialmente interpretadores, enquanto os sistemas **A-0/A-1/A-2** funcionavam de maneira mais próxima de expansores de macros, embora fossem chamados de "compiladores" na época.

---

## 4. O projeto Fortran e a confiança dos programadores

O projeto **Fortran** precisou convencer os programadores de que o código traduzido por um compilador poderia competir em desempenho com o código de máquina escrito à mão.

Na época, muitos programadores eram céticos e relutantes em abandonar a linguagem Assembly, pois temiam que o código gerado automaticamente fosse muito mais lento e ineficiente do que aquele produzido manualmente.

Além disso, os computadores eram caros e possuíam recursos limitados. Portanto, o desempenho do código executado era uma preocupação fundamental.

Para enfrentar esse problema, a equipe do Fortran investiu intensamente na criação de um compilador capaz de produzir código altamente eficiente. A ideia era reduzir o **custo e o tempo de programação** sem sacrificar significativamente o **desempenho da execução**.

Quando o compilador conseguiu produzir código cuja eficiência competia com o trabalho manual, o Fortran reduziu o receio dos programadores e tornou-se muito mais atraente para uso profissional.

Assim, o Fortran demonstrou que era possível obter uma combinação importante de:

* **alto desempenho**;
* **menor custo de programação**;
* **maior produtividade**;
* **redução de erros de programação**.

Essa combinação foi fundamental para sua adoção.

---

## 6. Contribuições do ALGOL 60

Três contribuições fundamentais do **ALGOL 60** ultrapassaram seu sucesso comercial e influenciaram fortemente o projeto de linguagens imperativas posteriores.

### 1. Estrutura de blocos

O ALGOL 60 introduziu uma organização baseada em **blocos**, permitindo a criação de escopos locais e ambientes de dados aninhados dentro do programa.

Esse conceito tornou possível organizar programas complexos de maneira mais estruturada, controlando melhor a visibilidade das variáveis.

### 2. Recursão

O ALGOL 60 permitiu que procedimentos fossem chamados **recursivamente**, possibilitando que uma função ou procedimento chamasse a si próprio.

A recursão se tornou um recurso fundamental para a solução de diversos problemas, principalmente aqueles que possuem uma estrutura naturalmente recursiva, como árvores e algoritmos de divisão e conquista.

### 3. BNF (Forma de Backus-Naur)

O ALGOL 60 teve sua sintaxe descrita formalmente utilizando a **BNF (Backus-Naur Form)**.

Esse recurso foi extremamente importante porque permitiu representar a estrutura sintática de uma linguagem de maneira precisa e formal, contribuindo para o desenvolvimento posterior dos estudos de análise sintática e dos compiladores.

### Influência sem domínio do mercado

Uma linguagem pode ser muito influente sem dominar o mercado porque seu valor histórico não depende apenas de sua popularidade comercial.

Uma linguagem pode funcionar como um **veículo de inovação conceitual**, introduzindo ideias que serão posteriormente incorporadas por outras linguagens mais populares.

Assim, mesmo que uma linguagem não tenha grande adoção comercial, suas ideias podem influenciar gerações posteriores de linguagens e ferramentas. O ALGOL 60 é um exemplo importante: apesar de não ter dominado o mercado, seus conceitos tiveram enorme influência no desenvolvimento das linguagens de programação posteriores.


15\. A primeira aplicação de Java não foi a Web, mas a Web impulsionou sua adoção. Explique como mudanças de contexto podem reposicionar uma linguagem.

R: Na década de 1990, o Java foi criado como uma linguagem confiável para sistemas embarcados e eletrônicos de consumo. Porém, seus primeiros produtos não chegaram ao mercado. Com a popularização da Web a partir de 1993, o Java ganhou destaque por ser útil no desenvolvimento para a Internet, principalmente por meio dos applets, pequenos programas executados nos navegadores. Assim, durante os primeiros anos de sua popularidade, a Web foi sua principal aplicação, fazendo com que o Java saísse de uma linguagem pouco popular e utilizada, para uma linguagem que vemos suas aplicações diariamente.

16\. Compare Perl, JavaScript, PHP, Python, Ruby e Lua usando três eixos: domínio inicial, estruturas de dados e estratégia de implementação. Evite concluir que todas são iguais por serem chamadas de scripting.

R: Perl: surgiu para processamento de texto e administração de sistemas; usa escalares, vetores e hashes; é compilada para uma representação intermediária.

JavaScript: nasceu para programação no navegador; usa strings, vetores e objetos baseados em protótipos; tradicionalmente é interpretada pelo navegador.

PHP: começou como ferramenta para páginas Web e evoluiu para aplicações no servidor; combina vetores e hashes; é interpretada no servidor.

Python: voltada inicialmente à administração de sistemas; utiliza listas, tuplas e dicionários; possui tipagem dinâmica, orientação a objetos e coleta de lixo.

Ruby: criada como linguagem de propósito geral e orientação a objetos; tudo é tratado como objeto e métodos podem ser adicionados dinamicamente.

Lua: desenvolvida para scripting e extensibilidade; baseada principalmente em uma única estrutura, a tabela, e é traduzida para código intermediário antes da interpretação.

17\. C# foi apresentada como evolução no ambiente .NET. Compare duas decisões de C# com suas correspondentes em Java ou C++ e explique o problema que pretendem resolver.

R: O C#, lançado pela Microsoft em 2000 como principal linguagem da plataforma .NET, foi inspirado em C++ e Java, mas introduziu melhorias para aumentar a segurança, simplicidade e expressividade. Duas decisões importantes foram os delegates que são referências seguras e orientadas a objetos para subprogramas. Substituem os ponteiros para funções inseguros do C++ e evitam a necessidade de interfaces complexas do Java. Facilitam callbacks, eventos e execução de threads, combinando flexibilidade com segurança. E boxing e unboxing C# unifica seu sistema de tipos fazendo com que todos os tipos derivem de System.Object. Permite converter valores primitivos em objetos (boxing) e recuperá-los (unboxing). Isso simplifica o uso de coleções e evita a necessidade de classes wrapper manuais.

18\. Diferencie XSLT e JSP quanto a entrada, processamento e saída. Por que ambas podem ser chamadas de linguagens híbridas de marcação e programação?

R: XSLT recebe XML, aplica regras de transformação e filtragem e gera uma nova saída, como XML, HTML ou texto.

JSTL/JS recebe requisições HTTP e parâmetros, executa lógica no servidor por meio de tags e gera HTML dinâmico para o navegador.

Ambas são consideradas linguagens híbridas, pois adicionam recursos de programação, como condicionais, loops e manipulação de dados, a linguagens de marcação que originalmente eram voltadas apenas à apresentação de informações.

19\. Crie uma linha do tempo com oito linguagens de pelo menos quatro paradigmas. Para cada ligação, escreva o tipo de influência; não use apenas setas cronológicas.

R:

1957 – Fortran: base da programação imperativa, com expressões matemáticas e loops.

1958 – Lisp: pioneira na programação funcional, com listas, condicionais e recursão.

1960 – ALGOL 60: introduziu blocos, escopo local, recursão e ortogonalidade, influenciando linguagens posteriores.

1967 – Simula 67: pioneira na orientação a objetos, com classes e herança.

1972 – Prolog: introduziu a programação lógica, baseada em fatos, regras e inferência.

1983 – C++: combinou eficiência de baixo nível do C com classes e herança, mas trouxe maior complexidade e problemas de segurança.

1995 – Java: buscou maior segurança e confiabilidade, eliminando ponteiros, usando coleta de lixo e verificação de limites.

2000 – C#: surgiu no .NET, refinando ideias do Java e adicionando recursos como structs e delegates.

20\. Estudo de caso: uma equipe precisa escolher tecnologias para cálculo científico, regras declarativas, aplicação Web interativa e firmware restrito. Proponha famílias de linguagens, justifique historicamente cada escolha e explicite dois trade-offs.

R:

Cálculo científico → Fortran: eficiente e otimizado graças aos tipos e armazenamento estáticos.

Regras declarativas → Prolog: baseado em fatos e regras, com execução determinada pelo sistema de inferência.

Web interativa → JavaScript/PHP: JavaScript atua no cliente e PHP no servidor.

Firmware restrito → C/C++: próximos ao hardware, geram código rápido e pequeno, com pouca sobrecarga de execução.

Trade-offs principais

Confiabilidade × Eficiência: Java/C# oferecem mais segurança, mas podem ter maior custo de execução. C prioriza velocidade, sacrificando segurança de memória.

Legibilidade × Facilidade de escrita: Linguagens mais expressivas permitem escrever menos código e desenvolver mais rápido, mas podem prejudicar a legibilidade e manutenção.