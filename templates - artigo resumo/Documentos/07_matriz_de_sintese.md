# Etapa 7 Matriz de síntese e organização da revisão

## Solicitação

Compare os artigos e organize a revisão por temas ou eixos. Não produza apenas uma sequência de resumos.

## Eixos da revisão

1. `[Complexidade computacional e eficiência de comunicação no Aprendizado Federado]`
2. `[Convergência do FedAvg e influência dos parâmetros de treinamento]`
3. `[Aplicação do Aprendizado Federado em classificação e análise de imagens médicas]`

## Matriz de síntese

| Eixo | Artigos relacionados | Convergências | Divergências | Limitações | Lacunas |
|---|---|---|---|---|---|
| `[Complexidade computacional e eficiência de comunicação no Aprendizado Federado]` | `[McMahan et al. (2017); Gao, Xu e Huang (2021); Cheng et al. (2023); Nanakaran e Ukwatta (2025); Eshwarappa et al. (2025); Le et al. (2026)]` | `[Os estudos apontam a comunicação como um dos principais gargalos e apresentam diferentes formas de reduzir esse custo.]` | `[As estratégias variam entre processamento local, compressão, treinamento em estágios, redução de dimensionalidade e edge computing.]` | `[Os estudos utilizam ambientes, modelos e distribuições de dados diferentes, dificultando comparações diretas.]` | `[Apesar dos avanços encontrados nos estudos sobre eficiência, convergência e aplicações médicas do Aprendizado Federado, ainda faltam análises que avaliem de forma conjunta e padronizada como o número de clientes, a quantidade de rodadas e o tamanho do modelo impactam os custos computacional e de comunicação do FedAvg em cenários de imagens médicas.]` |
| `[Convergência do FedAvg e influência dos parâmetros de treinamento]` | `[McMahan et al. (2017); Li et al. (2020); Gao, Xu e Huang (2021); Cheng et al. (2023); Nanakaran e Ukwatta (2025); Eshwarappa et al. (2025)]` | `[Os trabalhos mostram que heterogeneidade dos dados e parâmetros de treinamento influenciam a convergência e a comunicação.]` | `[Alguns estudos são mais teóricos, enquanto outros utilizam experimentos e aplicações médicas.]` | `[Parte dos resultados depende de condições matemáticas ou cenários simulados específicos.]` | `[Apesar dos avanços encontrados nos estudos sobre eficiência, convergência e aplicações médicas do Aprendizado Federado, ainda faltam análises que avaliem de forma conjunta e padronizada como o número de clientes, a quantidade de rodadas e o tamanho do modelo impactam os custos computacional e de comunicação do FedAvg em cenários de imagens médicas.]` |
| `[Aplicação do Aprendizado Federado em classificação e análise de imagens médicas]` | `[Sandhu et al. (2023); Nanakaran e Ukwatta (2025); Eshwarappa et al. (2025); Le et al. (2026)]` | `[Os estudos mostram que o Aprendizado Federado permite colaboração entre instituições sem centralizar os dados brutos.]` | `[Sandhu e Le são revisões; Nanakaran e Eshwarappa apresentam aplicações experimentais.]` | `[Os estudos utilizam diferentes modalidades médicas, cenários e infraestruturas.]` | `[Apesar dos avanços encontrados nos estudos sobre eficiência, convergência e aplicações médicas do Aprendizado Federado, ainda faltam análises que avaliem de forma conjunta e padronizada como o número de clientes, a quantidade de rodadas e o tamanho do modelo impactam os custos computacional e de comunicação do FedAvg em cenários de imagens médicas.]` |


## Roteiro da revisão da literatura

### Eixo 1

- Ideia principal: `[Entender como os estudos tentam reduzir o custo de processamento e principalmente de comunicação no Aprendizado Federado, olhando para fatores como processamento local, quantidade de rodadas e volume de dados enviados.]`
- Evidências que serão usadas: `[McMahan et al. mostra que o FedAvg consegue diminuir bastante o número de rodadas de comunicação. Gao, Xu e Huang apresenta o uso de compressão para reduzir o tráfego de dados. Cheng et al. propõe uma estratégia de treinamento que busca reduzir a comunicação sem prejudicar a convergência. Nanakaran e Ukwatta reduz o número de rodadas de 200 para 38, além de diminuir o tempo de treinamento e o consumo de energia. Eshwarappa et al. mostra redução de latência com o Edge-Avg, e Le et al. reforça que o custo de comunicação ainda é um dos desafios do Aprendizado Federado em imagens médicas.]`
- Comparação entre estudos: `[Os trabalhos têm o mesmo objetivo de melhorar a eficiência, mas seguem caminhos diferentes. Alguns focam em aumentar o processamento local, outros em reduzir a quantidade de dados transmitidos, diminuir o número de rodadas ou mudar a arquitetura usada no treinamento.]`
- Ligação com o problema: `[Esse eixo ajuda a entender melhor quais fatores podem aumentar ou diminuir os custos de processamento e comunicação do FedAvg, que são pontos centrais do nosso trabalho.]`

### Eixo 2

- Ideia principal: `[Analisar como os parâmetros do treinamento e as características dos dados podem influenciar a convergência e a eficiência do FedAvg.]`
- Evidências que serão usadas: `[Li et al. mostra que dados não-IID podem dificultar a convergência e que existe um equilíbrio na quantidade de passos locais. McMahan mostra que aumentar o processamento local pode reduzir a comunicação. Gao e Cheng apresentam estratégias para reduzir a comunicação mantendo uma boa convergência. Nanakaran utiliza early stopping para diminuir o número de rodadas, enquanto Eshwarappa mostra que a taxa de aprendizado pode afetar diretamente o desempenho e a estabilidade do modelo.]`
- Comparação entre estudos: `[Li trabalha mais com a parte teórica da convergência, enquanto McMahan apresenta resultados experimentais do FedAvg. Gao e Cheng propõem outras estratégias para melhorar a eficiência, e Nanakaran e Eshwarappa mostram esse tipo de problema em aplicações médicas.]`
- Ligação com o problema: `[Esse eixo mostra que número de clientes, quantidade de rodadas e processamento local estão ligados ao comportamento do modelo e não devem ser analisados separadamente.]`

### Eixo 3

- Ideia principal: `[Entender como o Aprendizado Federado vem sendo usado em imagens médicas e quais são os principais desafios encontrados nesse tipo de aplicação.]`
- Evidências que serão usadas: `[Sandhu et al. apresenta uma visão geral das aplicações de Aprendizado Federado em imagens médicas e mostra que o FedAvg aparece com frequência como técnica de agregação. Nanakaran e Ukwatta trabalha com ressonância magnética de próstata. Eshwarappa et al. utiliza imagens de câncer de pele. Le et al. destaca desafios como dados não-IID, comunicação, privacidade e agregação dos modelos.]`
- Comparação entre estudos: `[Sandhu e Le fazem revisões mais amplas sobre a área, enquanto Nanakaran e Eshwarappa apresentam aplicações práticas. Mesmo com abordagens diferentes, todos mostram que comunicação, heterogeneidade dos dados e privacidade são questões importantes em cenários médicos.]`
- Ligação com o problema: `[Esse eixo ajuda a justificar o uso de imagens médicas no nosso trabalho e mostra que os custos computacional e de comunicação também são importantes em ambientes com diferentes instituições e dados distribuídos.]`

## Síntese crítica provisória

`[A análise dos artigos mostra uma tendência de busca por maior eficiência no Aprendizado Federado, principalmente por meio da redução dos custos de comunicação e da otimização do processamento local. Embora os estudos utilizem estratégias diferentes, como compressão, aumento do processamento local, early stopping e edge computing, eles indicam que fatores como número de rodadas, quantidade de clientes e distribuição dos dados influenciam diretamente o treinamento. Também foi observado que os trabalhos utilizam diferentes modelos, bases de dados e cenários experimentais, o que dificulta uma comparação direta entre os resultados. Como principal lacuna, foram encontrados poucos estudos que avaliam de forma conjunta o impacto do número de clientes, da quantidade de rodadas e do tamanho do modelo sobre os custos computacional e de comunicação do FedAvg em aplicações com imagens médicas.]`

## Checklist

- [X] Os artigos foram agrupados por ideias.
- [X] Há comparações entre estudos.
- [X] As divergências foram registradas.
- [X] As lacunas são específicas e sustentadas pelas leituras.
