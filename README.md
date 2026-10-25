# Complexidade de Algoritmos em Aprendizado Federado: uma Análise do FedAvg para Classificação Distribuída de Imagens Médicas

> Projeto de pesquisa acadêmica desenvolvido no âmbito da disciplina de Computabilidade e Complexidade de Algoritmos, com foco na análise da complexidade computacional do algoritmo Federated Averaging (FedAvg) em aplicações de Aprendizado Federado para imagens médicas.

## Sobre o projeto

O Aprendizado Federado (Federated Learning – FL) permite que diferentes instituições participem do treinamento de um modelo sem a necessidade de centralizar seus dados brutos.

Na área da saúde, essa característica é especialmente relevante devido à sensibilidade das informações dos pacientes e à distribuição dos dados entre diferentes hospitais e centros médicos.

Entretanto, o treinamento federado apresenta desafios relacionados ao processamento local, à comunicação entre clientes e servidor, à convergência do modelo e à heterogeneidade dos dados.

Este projeto analisa esses desafios a partir do algoritmo **FedAvg**, considerando principalmente três variáveis:

- número de clientes participantes (`K`);
- quantidade de rodadas de comunicação (`R`);
- tamanho do modelo.

---

## Problema de pesquisa

> De que forma a variação do número de clientes (`K`), da quantidade de rodadas (`R`) e do tamanho do modelo impacta a complexidade computacional e os custos de comunicação do algoritmo FedAvg em cenários de classificação de imagens médicas?

---

## Objetivo geral

Analisar o impacto do número de clientes, da quantidade de rodadas de comunicação e do tamanho do modelo sobre a complexidade computacional e os custos de comunicação do FedAvg no contexto da classificação de imagens médicas.

---

## Objetivos específicos

- Conceituar o Aprendizado Federado e apresentar o funcionamento do FedAvg.
- Analisar os principais fatores relacionados à complexidade computacional do algoritmo.
- Investigar como o número de clientes e a quantidade de rodadas influenciam os custos do treinamento.
- Analisar a influência do tamanho do modelo sobre processamento e comunicação.
- Comparar estratégias utilizadas na literatura para melhorar a eficiência do treinamento federado.
- Identificar limitações e lacunas nas aplicações de FedAvg em imagens médicas.

---

## Metodologia

O trabalho foi desenvolvido como uma **revisão narrativa da literatura**, com abordagem qualitativa e caráter exploratório-analítico.

As buscas foram realizadas nas seguintes bases:

- PubMed / PMC;
- IEEE Xplore;
- ScienceDirect;
- Google Scholar.

Foram utilizadas combinações de termos relacionados a:

- `Federated Learning`;
- `FedAvg`;
- `Federated Averaging`;
- `Computational Complexity`;
- `Communication Cost`;
- `Rounds`;
- `Model Size`;
- `Medical Imaging`;
- `Medical Image Classification`.

A busca inicial identificou **44 trabalhos**. Após remoção de duplicatas, triagem e análise dos estudos, **8 artigos** foram selecionados para compor a revisão.

---

## Eixos da revisão da literatura

A análise dos trabalhos foi organizada em três eixos principais:

### 1. Complexidade computacional e eficiência de comunicação

Analisa o equilíbrio entre processamento local e comunicação, incluindo estratégias como compressão, redução de rodadas, redução de dimensionalidade e computação em borda.

### 2. Convergência do FedAvg e parâmetros de treinamento

Discute a influência de dados não-IID, passos locais, taxa de aprendizado, participação dos clientes e frequência de sincronização na convergência do FedAvg.

### 3. Aplicação em imagens médicas

Analisa aplicações do Aprendizado Federado em diferentes tipos de imagens médicas e os desafios relacionados à comunicação, heterogeneidade dos dados e infraestrutura.

---

## Principais resultados da revisão

A literatura analisada indica que não existe uma única configuração do FedAvg capaz de oferecer o melhor desempenho em todos os cenários.

Estratégias como:

- aumentar o processamento local;
- reduzir a frequência de sincronização;
- comprimir atualizações;
- reduzir a dimensionalidade dos dados;
- utilizar modelos mais compactos;
- utilizar computação em borda;

podem diminuir os custos de treinamento.

Entretanto, esses ganhos dependem da distribuição dos dados, da configuração dos parâmetros, da quantidade de clientes e da infraestrutura disponível.

A principal lacuna encontrada está na falta de estudos padronizados que avaliem conjuntamente o **número de clientes, a quantidade de rodadas e o tamanho do modelo** em aplicações de classificação de imagens médicas.

---
## Etapas do projeto

- [x] Definição do tema
- [x] Definição do problema de pesquisa
- [x] Definição dos objetivos
- [x] Planejamento das buscas
- [x] Levantamento bibliográfico
- [x] Triagem dos artigos
- [x] Leitura e fichamento
- [x] Matriz de síntese
- [x] Redação do artigo
- [x] Normalização e revisão
- [ ] Apresentação final

---

## Tecnologias e conceitos abordados

`Federated Learning` · `FedAvg` · `Machine Learning` · `Deep Learning` · `Complexidade de Algoritmos` · `Comunicação Distribuída` · `Medical Imaging`

---

## Integrantes
---
| Integrante | GitHub |
|---|---|
| Gabriel Anastácio Pereira | [@gabpereiraa](https://github.com/gabpereiraa) |
| Gabriel Alves Dias Reis | [@gabe-herrera](https://github.com/gabe-herrera) |
| Karen Gabrielle Justino | [@karenjustino](https://github.com/karenjustino) |
| Marcos Antonio da Silva Souza | [@MacQueenDev](https://github.com/MacQueenDev) |
| Matheus Silva Soares | [@mthxssoares](https://github.com/mthxssoares) |

---

## Informações acadêmicas

**Curso:** Ciência da Computação  
**Disciplina:** Computabilidade e Complexidade de Algoritmos  
**Projeto:** Mostra de Tecnologia 2026.2  
**Orientadora:** Profª Drª Andréa Ono Sakai  
**Grupo:** Grupo 7 — CC Noite

---

## Status

📚 **Pesquisa bibliográfica e redação do artigo concluídas.**

O projeto encontra-se atualmente na etapa de revisão final e preparação da apresentação acadêmica.