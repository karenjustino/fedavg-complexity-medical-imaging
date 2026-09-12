# Template de Definição de Objetivos da Pesquisa Científica
### Computabilidade e Complexidade de Algoritmos

> **Como usar este template:** respondam cada pergunta no espaço indicado por `> Resposta:`. Sigam o passo a passo e usem os exemplos apenas como referência de estrutura — o conteúdo deve ser sobre o tema do grupo.

---

## Identificação do Grupo


| Campo | Informação |
|---|---|
| Curso / Disciplina | `[Ciência da Computação — Computabilidade e Complexidade de Algoritmos]` |
| Projeto de Pesquisa / IC | `[Projeto de pesquisa Mostra de Tecnologia 2026.2]` |
| Orientador(a) | `[Profª Dorª Andréa Ono Sakai]` |
| Data de entrega desta etapa | `[dd/mm/aaaa]` |
| Integrantes do grupo | `[Gabriel Anastácio Pereira,Gabriel Alves Dias Reis, Karen Gabrielle Justino, Marcos Antonio da Silva Souza, Matheus Silva Soares]` |
| Tema (da etapa "a") | `[Complexidade computacional e de comunicação do FedAvg em cenarios simulados de apredindizado federado para classificação de imagens médicas]` |

---

## PARTE 1 — DEFINIR O OBJETIVO GERAL

### 1.1 Tema específico do grupo

**Pergunta:** Qual foi o tema específico que o grupo definiu?

> Resposta: Complexidade computacional e de comunicação do FedAvg em cenários simulados de aprendizado federado para classificação de imagens médicas.

### 1.2 Passo a passo para chegar ao objetivo geral

**Passo 1 — Delimitação do tema**
Delimitem o tema específico por área, tempo, espaço ou aplicação.

> Resposta: A pesquisa está delimitada à aplicação do algoritmo FedAvg no contexto de Aprendizado Federado voltado para a classificação de imagens médicas. No escopo técnico (espaço/aplicação), o estudo restringe-se a cenários simulados, analisando de forma separada as métricas de computação, comunicação, convergência e custo. Além disso, a abordagem delimita a questão da privacidade dos dados estritamente como um mecanismo de redução de risco (não como garantia absoluta) e exclui a classificação de ameaças bizantinas como P/NP sem formulação matemática e prova.

**Passo 2 — Formulação da problemática**
Transformem o tema em uma pergunta que expresse o problema de pesquisa.

> Resposta: De que forma a variação de parâmetros, como o número de clientes (K) e a quantidade de rodadas (R), impacta separadamente a complexidade computacional e os custos de comunicação do algoritmo FedAvg em simulações de imagens médicas?

**Passo 3 — Transformar a pergunta em objetivo geral**
Reescrevam a pergunta como uma afirmação, usando um verbo no infinitivo.

*Exemplo:* "Analisar os principais impactos da árvore de decisão em IA para definir estratégias de marketing para segmentação de clientes."

> Resposta:Avaliar, de forma separada, o impacto do número de clientes, da quantidade de rodadas e do tamanho do modelo sobre as complexidades computacional e de comunicação do algoritmo FedAvg, em cenários simulados de classificação distribuída de imagens médicas. Por que ela vai gostar? Porque você usa a expressão "de forma separada" (ou isolada), atendendo exatamente ao que ela escreveu na planilha: "separar computação, comunicação, convergência e custo".

**Passo 4 — Ajustes finais**
Revisem o objetivo geral seguindo os critérios abaixo:

- [x] É claro, direto e mensurável?
- [x] Evitei verbos fracos como "estudar" ou "conhecer"?
- [x] Usei um verbo forte (explorar, analisar, investigar, compreender, avaliar, propor, desenvolver, aplicar, identificar)?

**Modelo genérico de referência:**
> "[Verbo no infinitivo] a aplicação de [conceito ou técnica] em [contexto específico], com o propósito de [finalidade principal]."

**Outros exemplos de objetivos gerais (referência):**
- Investigar o uso de árvores de decisão para prever exportações de vinho no Brasil, com base em dados da Embrapa entre 2000 e 2025.
- Analisar o impacto da classificação automática de vinhos finos e de mesa por meio de algoritmos de inteligência artificial, a fim de apoiar estratégias de exportação.
- Desenvolver um modelo computacional baseado em árvore binária de busca para otimizar a recomendação de rotas de ambulância em cenários urbanos.

### 1.3 Respostas finais da Parte 1

**1) Qual a problemática?**

> Resposta:Como a complexidade algorítmica do Aprendizado Federado influencia o custo computacional e de comunicação em servidores Cloud utilizados para o diagnóstico por imagens médicas, sem comprometer a segurança dos dados sensíveis?

**2) Qual o objetivo geral?**

> Resposta: Avaliar o impacto do número de clientes, da quantidade de rodadas e do tamanho do modelo sobre a complexidade computacional, o custo de comunicação e a convergência do algoritmo FedAvg em cenários simulados de classificação de imagens médicas, considerando o uso de infraestrutura Cloud e os requisitos de segurança e privacidade dos dados.

---

## PARTE 2 — DEFININDO OS OBJETIVOS ESPECÍFICOS

### 2.1 Objetivo geral pesquisado

Copiem aqui o objetivo geral definido na Parte 1 (deve conceituar os assuntos abordados no tema).

> Resposta: Avaliar o impacto do número de clientes, da quantidade de rodadas e do tamanho do modelo sobre a complexidade computacional, o custo de comunicação e a convergência do algoritmo FedAvg em cenários simulados de classificação de imagens médicas, considerando o uso de infraestrutura Cloud e os requisitos de segurança e privacidade dos dados.

### 2.2 Assuntos da pesquisa

Escrevam de 4 a 5 assuntos que serão abordados na pesquisa.

*Exemplo (para o tema de árvore de decisão em IA e marketing):*
- Conceituar árvore de decisão
- Conceituar inteligência artificial
- Quais são as estratégias de marketing para segmentação de clientes?
- Analisar a relação existente entre árvore de decisão e inteligência artificial
- Apresentar quais são os resultados das estratégias de marketing para segmentação de clientes sem e com IA

**Assuntos do grupo:**
1. Resposta: Conceituar o Aprendizado Federado e a estrutura de funcionamento do algoritmo FedAvg.
2. Resposta: Analisar e separar matematicamente a complexidade computacional, a complexidade de comunicação e a taxa de convergência do FedAvg
3. Resposta: Mapear as métricas de complexidade na literatura, separando o custo computacional (tempo por rodada) do custo de comunicação (bytes transmitidos
4. Resposta: Avaliar a relação entre a complexidade algorítmica exigida e a convergência do modelo em ambientes simulados


### 2.3 Estrutura básica do artigo

Definam a estrutura do artigo, incluindo introdução e considerações finais.

*Exemplo de estrutura:*
- Introdução
- Conceituar árvore de decisão
- Conceituar inteligência artificial
- Quais são as estratégias de marketing para segmentação de clientes
- Analisar a relação existente entre árvore de decisão e inteligência artificial
- Apresentar quais são os resultados das estratégias de marketing para segmentação de clientes sem e com IA
- Considerações finais

**Estrutura do grupo:**
- Introdução
- Resposta: Fundamentos de Aprendizado Federado e funcionamento do FedAvg
- Resposta: Complexidade computacional aplicada ao FedAvg
- Resposta: Custo de comunicação no treinamento federado
- Resposta: Convergência do FedAvg e relação com o custo computacional e de comunicação
- Resposta: Impacto do número de clientes, quantidade de rodadas e tamanho do modelo
- Resposta: Análise dos resultados em cenários simulados de classificação de imagens médicas
- Considerações finais

### 2.4 Objetivos específicos classificados

Classifiquem os objetivos específicos em **Conceituais** e **Técnicos**.

*Exemplo:*
- **Objetivos Conceituais**
  - Conceituar árvore de decisão
  - Conceituar inteligência artificial 
- **Objetivos Técnicos**
  - Quais são as estratégias de marketing para segmentação de clientes
  - Analisar a relação existente entre árvore de decisão e inteligência artificial
  - Apresentar quais são os resultados das estratégias de marketing para segmentação de clientes sem e com IA

**Objetivos específicos do grupo:**

- **Objetivos Conceituais**
  - Resposta: Conceituar o Aprendizado Federado e descrever o funcionamento do algoritmo FedAvg.
  - Resposta: Apresentar os conceitos de complexidade computacional, complexidade de comunicação, convergência, Cloud Computing e privacidade aplicados ao contexto do Aprendizado Federado.

- **Objetivos Técnicos**
  - Resposta: Analisar o impacto do número de clientes, da quantidade de rodadas e do tamanho do modelo sobre o custo computacional e de comunicação do FedAvg.
  - Resposta: Comparar separadamente as métricas de processamento, comunicação e convergência nos cenários simulados.
  - Resposta: Avaliar a relação entre o uso de infraestrutura Cloud, o desempenho do treinamento federado e os mecanismos de segurança e privacidade aplicados aos dados médicos.

---

## CHECKLIST FINAL DO GRUPO

- [X] O tema específico está delimitado (área, tempo, espaço ou aplicação)
- [X] A problemática está formulada como pergunta
- [X] O objetivo geral está no infinitivo, claro e mensurável
- [X] Foram listados de 4 a 5 assuntos do artigo
- [X] A estrutura do artigo foi definida (introdução, desenvolvimento, considerações finais)
- [X] Os objetivos específicos foram classificados em Conceituais e Técnicos


