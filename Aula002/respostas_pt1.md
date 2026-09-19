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