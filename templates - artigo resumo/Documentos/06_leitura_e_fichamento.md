# Etapa 6 Leitura e fichamento

## Solicitação

Preencha uma cópia deste template para cada artigo selecionado.

## Artigo 1 — McMahan et al. (2017)
## Identificação do artigo

- Referência completa: `[MCMAHAN, H. Brendan; MOORE, Eider; RAMAGE, Daniel; HAMPSON, Seth; AGUERA Y ARCAS, Blaise. Communication-efficient learning of deep networks from decentralized data. Proceedings of the 20th International Conference on Artificial Intelligence and Statistics, v. 54, p. 1273–1282, 2017.]`
- DOI ou URL: `[https://proceedings.mlr.press/v54/mcmahan17a.html]`
- Base de origem: `[Google Scholar / PMLR]`
- Leitor responsável: `[Matheus silva Soares]`
- Data da leitura: `[08/10/2026]`

## Fichamento

### Problema investigado

`[O estudo investiga como treinar modelos de aprendizado de máquina utilizando dados descentralizados em dispositivos de usuários sem a necessidade de transferir os dados brutos para um servidor central. O principal desafio considerado é o alto custo de comunicação entre clientes e servidor, além das características típicas do cenário federado, como dados não-IID, desbalanceados e distribuídos entre muitos clientes.]`

### Objetivo do estudo

`[Propor e avaliar uma abordagem prática de Aprendizado Federado capaz de treinar redes neurais profundas sobre dados descentralizados, reduzindo principalmente a quantidade de rodadas de comunicação necessárias entre os clientes e o servidor.]`

### Método utilizado

`[Os autores desenvolveram o algoritmo FederatedAveraging (FedAvg), no qual uma fração dos clientes é selecionada a cada rodada, recebe o modelo global, realiza treinamento local utilizando SGD e envia o modelo atualizado ao servidor. O servidor então realiza uma média ponderada das atualizações recebidas para gerar uma nova versão do modelo global. Os experimentos variaram principalmente a fração de clientes participantes (C), o número de épocas locais (E) e o tamanho do minibatch local (B).]`

### Contexto, amostra ou dados

`[A avaliação experimental considerou cinco arquiteturas de modelos e quatro conjuntos de dados, incluindo tarefas de classificação de imagens e modelagem de linguagem. Foram utilizados MNIST para reconhecimento de dígitos, CIFAR-10 para classificação de imagens e conjuntos de dados relacionados a Shakespeare e previsão de palavras. Os experimentos também consideraram distribuições IID e não-IID, além de conjuntos de dados desbalanceados entre os clientes.]`

### Principais resultados

`[Os resultados demonstraram que o FedAvg pode reduzir significativamente a quantidade de rodadas de comunicação necessárias para o treinamento. Os autores relatam uma redução de aproximadamente 10 a 100 vezes no número de rodadas de comunicação em comparação com o FederatedSGD sincronizado. Os experimentos também mostram que realizar mais processamento local antes da comunicação pode aumentar a eficiência do treinamento, mantendo bom desempenho mesmo em situações com dados não-IID e desbalanceados.]`

### Limitações apresentadas

`[O estudo foi realizado em um ambiente experimental controlado e não contempla todos os problemas encontrados em uma implementação federada real. Os autores citam como questões fora do escopo a variação dos dados locais ao longo do tempo, diferenças na disponibilidade dos clientes, clientes que não respondem e atualizações corrompidas. O trabalho também não apresenta uma solução completa de privacidade e segurança, indicando mecanismos como privacidade diferencial e computação multipartidária segura como possibilidades complementares.]`

### Contribuição para o nosso artigo

`[O estudo contribui diretamente para a nossa pesquisa porque apresenta o algoritmo FedAvg e demonstra a relação entre computação local e custo de comunicação. Ele ajuda a compreender como o aumento do processamento realizado pelos clientes pode reduzir a quantidade de rodadas necessárias entre clientes e servidor. Além disso, o artigo analisa a participação de diferentes quantidades de clientes e o treinamento realizado ao longo de rodadas, elementos diretamente relacionados ao problema de pesquisa do grupo.]`

### Comentário crítico

`[O artigo apresenta como principal ponto forte a proposta de um algoritmo simples e prático para o treinamento federado, acompanhado de experimentos em diferentes modelos, bases de dados e distribuições de dados. Outro aspecto positivo é a análise do equilíbrio entre processamento local e comunicação. Como limitação, os experimentos não representam todas as condições de um ambiente federado real, e questões de segurança e privacidade são discutidas apenas de forma complementar. Mesmo assim, o estudo constitui uma referência fundamental para compreender o funcionamento e a eficiência do FedAvg.]`

### Citação literal opcional

> `["Communication costs are the principal constraint."]`

Página: `[1 do PDF / p. 1273 dos anais]`

## Artigo 2 — Li et al. (2020)
## Identificação do artigo

- Referência completa: `[LI, Xiang; HUANG, Kaixuan; YANG, Wenhao; WANG, Shusen; ZHANG, Zhihua. On the convergence of FedAvg on non-IID data. International Conference on Learning Representations – ICLR, 2020.]`
- DOI ou URL: `[https://arxiv.org/abs/1907.02189]`
- Base de origem: `[Google Scholar / arXiv]`
- Leitor responsável: `[Karen Gabrielle Justino]`
- Data da leitura: `[09/10/2026]`

## Fichamento

### Problema investigado

`[A principal lacuna investigada é a falta de garantias teóricas de convergência para o FedAvg em cenários realistas, onde os dados são heterogêneos (não-IID) e apenas parte dos dispositivos participa. O estudo busca estabelecer a taxa de convergência do FedAvg para problemas fortemente convexos e suaves sem depender de suposições idealizadas.]`

### Objetivo do estudo

`[Analisar teoricamente a convergência do algoritmo Federated Averaging (FedAvg) em cenários de dados heterogêneos (não-IID) para problemas fortemente convexos e suaves. O estudo visa eliminar suposições idealizadas da literatura, como distribuição IID e participação integral dos dispositivos, e estabelecer formalmente uma taxa de convergência de O(1/T) sob condições realistas.]`

### Método utilizado

`[Abordagem teórico-metodológica baseada em modelagem matemática e análise formal de otimização convexa, complementada por validação experimental computacional para corroborar os limites teóricos estabelecidos para o algoritmo.]`

### Contexto, amostra ou dados

`[O estudo utiliza simulações computacionais distribuídas com N = 100 dispositivos simulados. Foram empregados o conjunto MNIST particionado de forma não-IID, em configurações balanceadas e desbalanceadas, além de conjuntos de dados sintéticos para controlar a heterogeneidade. Também foi utilizada uma formulação analítica com regressão Ridge para parte da análise teórica.]`

### Principais resultados

`[O FedAvg alcançou taxa de convergência teórica de O(1/T) para funções suaves e fortemente convexas, mesmo em condições não-IID e com participação parcial dos dispositivos. O estudo também identificou a existência de um número adequado de passos locais: poucos passos aumentam a comunicação, enquanto passos excessivos podem prejudicar a convergência. A taxa de aprendizado decrescente mostrou-se necessária para garantir a convergência. Os experimentos com diferentes quantidades de clientes também indicaram que aumentar o número de nós ativos produz ganhos apenas marginais em determinadas condições.]`

### Limitações apresentadas

`[As garantias teóricas concentram-se em problemas fortemente convexos e suaves, não abrangendo diretamente modelos não convexos complexos, como redes neurais profundas. O estudo também depende de determinadas hipóteses de amostragem e identifica limitações relacionadas ao número de passos locais e à ausência de aceleração linear com o aumento do número de clientes.]`

### Contribuição para o nosso artigo

`[Este estudo contribui para o nosso artigo ao demonstrar teoricamente como o FedAvg equilibra o custo de comunicação e o processamento local em situações com dados não-IID. Os resultados ajudam a compreender como a quantidade de passos locais, a participação dos clientes e a heterogeneidade dos dados influenciam a convergência e a necessidade de comunicação, aspectos diretamente relacionados ao número de clientes e de rodadas analisados em nossa pesquisa.]`

### Comentário crítico

`[[O estudo apresenta como principal ponto forte uma análise matemática rigorosa da convergência do FedAvg em dados não-IID e com participação parcial dos clientes. Entretanto, suas garantias estão restritas principalmente a problemas convexos e não representam integralmente redes neurais profundas. Apesar dessa limitação, o trabalho fornece uma base teórica importante para compreender o equilíbrio entre computação local, comunicação e convergência.]`

### Citação literal opcional

> `["heterogeneity of data slows down the convergence"]`

Página: `[1 do PDF]`
## Artigo 3 — Gao, Xu e Huang (2021)
## Identificação do artigo

- Referência completa: `[GAO, Hongchang; XU, An; HUANG, Heng. On the convergence of communication-efficient Local SGD for Federated Learning. Proceedings of the AAAI Conference on Artificial Intelligence, v. 35, n. 9, p. 7510–7518, 2021.]`
- DOI ou URL: `[https://doi.org/10.1609/aaai.v35i9.16920]`
- Base de origem: `[Google Scholar / AAAI]`
- Leitor responsável: `[Karen Gabrielle Justino]`
- Data da leitura: `[09/10/2026]`

## Fichamento

### Problema investigado

`[O estudo investiga como integrar compressão bidirecional com compensação de erro ao Local SGD, tanto na versão padrão quanto com momentum, para reduzir os custos de comunicação nos sentidos cliente-servidor e servidor-cliente, sem comprometer a taxa de convergência.]`

### Objetivo do estudo

`[Propor e analisar teoricamente novos métodos de Local SGD eficientes em comunicação para Aprendizado Federado, utilizando compressão bidirecional com compensação de erro em problemas não convexos, buscando reduzir a transferência de dados sem prejudicar a convergência.]`

### Método utilizado

`[O estudo combina análise matemática de convergência com experimentos computacionais. Os autores propõem métodos de Local SGD e Momentum Local SGD utilizando compressão de gradientes e compensação de erro. Os testes foram realizados em PyTorch, utilizando CIFAR-10 com ResNet-56 e ImageNet com ResNet-50, além de diferentes intervalos de sincronização.]`

### Contexto, amostra ou dados

`[Foram utilizados os conjuntos de dados CIFAR-10 e ImageNet com os modelos ResNet-56 e ResNet-50, respectivamente. Os experimentos foram executados em um cluster com oito GPUs NVIDIA Tesla P40 e utilizaram distribuição IID dos dados e compressão por esparsificação top-10%.]`

### Principais resultados

`[Os métodos propostos reduziram significativamente o tráfego de dados sem comprometer de forma relevante o desempenho dos modelos. Teoricamente, os algoritmos mantiveram taxa de convergência O(1/√KT) com aceleração linear. Nos experimentos, as versões comprimidas apresentaram acurácias próximas às versões de precisão completa, mesmo utilizando menor quantidade de dados transmitidos.]`

### Limitações apresentadas

`[O principal limite do estudo é considerar dados distribuídos de forma IID na análise principal. Além disso, os experimentos foram realizados em um cluster controlado, não contemplando integralmente situações reais de Aprendizado Federado, como clientes lentos, desconexões e restrições severas de largura de banda.]`

### Contribuição para o nosso artigo

`[O estudo contribui ao mostrar que o custo de comunicação não depende somente do número de rodadas, mas também do volume de informação transmitido em cada sincronização. A utilização de compressão demonstra uma forma de reduzir esse custo mantendo a convergência, ajudando a fundamentar a análise da relação entre tamanho do modelo, quantidade de clientes e comunicação.]`

### Comentário crítico

`[O estudo apresenta como pontos fortes a fundamentação matemática e a validação em redes neurais profundas. A compressão bidirecional demonstra potencial para reduzir significativamente o tráfego de comunicação. Entretanto, a utilização de dados IID e de uma infraestrutura controlada limita a generalização dos resultados para cenários federados reais, nos quais dados não-IID e diferenças entre dispositivos são frequentes.]`

### Citação literal opcional

> `["significantly reduce the communication cost"]`

Página: `[1 do PDF / p. 7510 dos anais]`
## Artigo 4 — Sandhu et al. (2023)
## Identificação do artigo

- Referência completa: `[SANDHU, Sukhveer Singh et al. Medical Imaging Applications of Federated Learning. Diagnostics, v. 13, n. 19, art. 3140, 2023.]`
- DOI ou URL: `[https://doi.org/10.3390/diagnostics13193140]`
- Base de origem: `[PubMed / Google Scholar]`
- Leitor responsável: `[Marcos Antonio da Silva Souza]`
- Data da leitura: `[08/10/2026]`

## Fichamento

### Problema investigado

`[O estudo investiga os desafios relacionados ao uso de dados médicos para o treinamento de modelos de aprendizado de máquina, principalmente devido à necessidade de preservar a privacidade dos pacientes e às restrições legais para compartilhamento de informações. Além disso, os dados médicos podem apresentar diferentes características entre instituições, o que dificulta a criação de modelos capazes de generalizar adequadamente.]`

### Objetivo do estudo

`[O objetivo é analisar o estado atual da aplicação do Federated Learning em imagens médicas, investigando seus fluxos de trabalho, arquiteturas, algoritmos e estruturas utilizadas. O estudo também busca identificar os principais cenários e tarefas em que o aprendizado federado é aplicado na área de imagens médicas.]`

### Método utilizado

`[Os autores realizaram uma revisão sistemática da literatura sobre aplicações de Federated Learning em imagens médicas. A análise considera diferentes estudos e aplicações, comparando abordagens de aprendizado centralizado e federado e observando aspectos relacionados aos métodos de treinamento, agregação dos modelos, privacidade e características dos dados.]`

### Contexto, amostra ou dados

`[O estudo está inserido no contexto da inteligência artificial aplicada à área da saúde, especialmente no processamento e análise de imagens médicas. São considerados trabalhos relacionados a diferentes regiões do corpo e doenças, incluindo aplicações envolvendo cérebro, mama, pâncreas, próstata e COVID-19. Os estudos analisados utilizam diferentes tipos de imagens e tarefas de aprendizado de máquina.]`

### Principais resultados

`[Os resultados mostram que o Federated Learning permite que diferentes instituições treinem um modelo de forma colaborativa sem precisar compartilhar diretamente os dados médicos brutos. Em vez disso, os modelos ou seus parâmetros são compartilhados e agregados. O FedAvg aparece como uma das técnicas de agregação mais utilizadas. Os estudos analisados também indicam que modelos federados podem apresentar desempenho comparável ao aprendizado centralizado, além de oferecerem vantagens relacionadas à privacidade dos dados.]`

### Limitações apresentadas

`[Entre as principais limitações estão as diferenças na distribuição dos dados entre as instituições, conhecidas como características não-IID, além de questões relacionadas à segurança, comunicação, recursos computacionais e dificuldade para estabelecer parcerias entre diferentes instituições. Os autores também destacam que o Federated Learning precisa ser adaptado às características específicas de cada tipo de imagem médica e doença.]`

### Contribuição para o nosso artigo

`[Este estudo contribui para o nosso artigo ao apresentar evidências de que o Federated Learning pode ser utilizado para desenvolver modelos de inteligência artificial em ambientes de saúde sem exigir o compartilhamento direto dos dados dos pacientes. Dessa forma, ele ajuda a fundamentar a utilização do aprendizado federado como uma alternativa para permitir a colaboração entre instituições, mantendo os dados localmente e contribuindo para a preservação da privacidade.]`

### Comentário crítico

`[O principal ponto positivo do estudo é sua abordagem ampla sobre diferentes aplicações do Federated Learning em imagens médicas, permitindo compreender tanto seus benefícios quanto seus desafios. Entretanto, a grande variedade de aplicações e características dos dados analisados dificulta estabelecer uma solução única para todos os cenários. Mesmo assim, o estudo apresenta uma contribuição relevante ao demonstrar que o aprendizado federado pode aproximar os benefícios do treinamento colaborativo dos benefícios do aprendizado centralizado, reduzindo a necessidade de compartilhamento direto de dados médicos.]`

### Citação literal opcional

> `[“FL boasts the ability to train a model collaboratively without requiring all the clients to have access to each other’s data while still reaping the benefits of a model that has seen all the data.”]`

Página: `[Página: 21]`
## Artigo 5 — Cheng et al. (2023)
## Identificação do artigo

- Referência completa: `[CHENG, Yifei et al. Communication-efficient federated learning with stagewise training strategy. Neural Networks, v. 167, p. 460–472, 2023.]`
- DOI ou URL: `[https://doi.org/10.1016/j.neunet.2023.08.033]`
- Base de origem: `[ScienceDirect / Google Scholar]`
- Leitor responsável: `[Gabriel Alves Dias Reis]`
- Data da leitura: `[09/10/2026]`

## Fichamento

### Problema investigado

`[O estudo investiga como reduzir o custo de comunicação entre os participantes (workers) durante o treinamento em aprendizado federado, especialmente quando os dados de cada participante são diferentes entre si (dados não IID). Nesse cenário, os métodos existentes tinham dificuldade para alcançar, ao mesmo tempo, uma boa velocidade de convergência e poucas rodadas de comunicação.]`

### Objetivo do estudo

`[Propor e analisar o SQUARFA, um algoritmo que busca reduzir a comunicação no aprendizado federado sem comprometer a convergência do treinamento. Os autores também investigam o uso da estratégia em diferentes tipos de problemas e em configurações com lotes maiores.]`

### Método utilizado

`[Os autores propõem um método de otimização que combina treinamento por etapas (stagewise training) com redução de variância. O algoritmo também usa uma fase inicial de partida rápida (quick-start) em cada etapa. O estudo apresenta análises teóricas sobre convergência e complexidade de comunicação e realiza experimentos comparando os algoritmos propostos com métodos de referência.]`

### Contexto, amostra ou dados

`[O contexto é o aprendizado federado, no qual os dados permanecem distribuídos entre diferentes participantes, em vez de serem reunidos em um único local. O artigo considera situações em que as distribuições de dados dos participantes não são iguais (não IID). Nos experimentos, os autores avaliam problemas convexos, incluindo regressão logística, e problemas não convexos, incluindo redes neurais. O resumo consultado não informa os nomes dos conjuntos de dados nem o tamanho da amostra, então esses detalhes precisam ser conferidos no texto integral.]`

### Principais resultados

`[Segundo os autores, a análise teórica mostra que o SQUARFA pode alcançar simultaneamente resultados favoráveis de convergência e de complexidade de comunicação para objetivos fortemente convexos e para objetivos não convexos que satisfazem a condição PL. O artigo também apresenta uma variante para objetivos não convexos gerais e estende a técnica para cenários de lotes grandes. Nos experimentos, os autores relatam desempenho superior dos algoritmos propostos em relação aos métodos comparados.]`

### Limitações apresentadas

`[Não identifiquei uma seção de limitações explícitas no resumo e no trecho do artigo consultado. Uma ressalva para a leitura é que parte importante da contribuição é teórica e depende de condições matemáticas específicas, como convexidade forte ou condição PL. Além disso, os resultados experimentais citados no resumo não permitem, por si só, concluir que o método terá o mesmo desempenho em qualquer aplicação real. Essa ressalva é uma avaliação crítica, não uma limitação declarada pelos autores.]`

### Contribuição para o nosso artigo

`[Se o artigo de vocês trata de aprendizado federado, otimização ou redução de custos de comunicação, este estudo pode servir como referência sobre o uso de treinamento por etapas e redução de variância para lidar com dados não IID.Se a revisão de vocês é especificamente sobre o caixeiro-viajante, a contribuição deste artigo parece indireta ou inexistente: o trabalho não investiga esse problema. Nesse caso, é melhor confirmar com a professora se ele realmente faz parte do conjunto de estudos da revisão.]`

### Comentário crítico

`[Um ponto forte do estudo é combinar análise teórica e experimentos, além de tratar diretamente uma dificuldade relevante do aprendizado federado: a diferença entre os dados dos participantes. Também é interessante que os autores busquem melhorar simultaneamente a convergência e a comunicação, em vez de tratar apenas uma dessas dimensões.Como ressalva, os resultados dependem das hipóteses e das configurações estudadas. Para avaliar melhor a aplicação prática, seria importante verificar no texto integral quais conjuntos de dados foram usados, quais métodos serviram de comparação e quanto o algoritmo reduziu a comunicação em cada experimento.]`

### Citação literal opcional

> `[The efficiency of communication across workers is a significant factor that affects the performance of federated learning.]`

Página: `[460]`
## Artigo 6 — Nanakaran e Ukwatta (2025)
## Identificação do artigo

- Referência completa: `[NANAKARAN, Negin Piran; UKWATTA, Eranga. A novel federated learning framework for medical imaging: resource-efficient approach combining PCA with early stopping. Medical Physics, v. 52, n. 8, e18064, 2025.]`
- DOI ou URL: `[https://doi.org/10.1002/mp.18064]`
- Base de origem: `[PubMed / PMC / Google Scholar]`
- Leitor responsável: `[Karen Gabrielle Justino]`
- Data da leitura: `[10/10/2026]`

## Fichamento

### Problema investigado

`[O estudo investiga como superar limitações de eficiência computacional e de comunicação do Aprendizado Federado aplicado a imagens médicas. O FedAvg convencional pode enfrentar custos elevados devido à alta dimensionalidade das imagens, às sincronizações frequentes e à heterogeneidade dos dados entre instituições.]`

### Objetivo do estudo

`[Avaliar um framework adaptativo de Aprendizado Federado para melhorar a eficiência computacional e de comunicação na classificação distribuída de imagens médicas, reduzindo os efeitos de dados não-IID e das limitações de infraestrutura.]`

### Método utilizado

`[Foi realizado um estudo quantitativo multicêntrico utilizando 1.500 exames de ressonância magnética. A abordagem combina Análise de Componentes Principais Incremental Federada (FIPCA), uma rede neural para classificação e um mecanismo adaptativo de early stopping, executados em ambiente federado utilizando o framework Flower.]`

### Contexto, amostra ou dados

`[Foram utilizados 1.500 exames de ressonância magnética da próstata provenientes do conjunto PI-CAI. Os dados foram distribuídos entre diferentes instituições para representar um cenário clínico descentralizado e não-IID. Dois centros foram utilizados para treinamento e validação e um terceiro centro independente foi utilizado exclusivamente para teste.]`

### Principais resultados

`[O framework proposto alcançou AUC de 0,733, superior ao FedAvg convencional, que apresentou 0,685, e próximo ao aprendizado centralizado, com 0,749. A combinação de FIPCA e early stopping reduziu as rodadas globais de 200 para 38, diminuiu o tempo de treinamento de 300 para 5 minutos e reduziu o consumo energético em até 98% em comparação com o FedAvg tradicional.]`

### Limitações apresentadas

`[A avaliação foi realizada em uma aplicação específica de classificação de câncer de próstata utilizando imagens de ressonância magnética e um número limitado de instituições. Além disso, a abordagem depende da redução linear de dimensionalidade por PCA e de uma quantidade mínima de dados disponíveis em cada centro, o que limita a generalização direta dos resultados para outras modalidades de imagem e contextos clínicos.]`

### Contribuição para o nosso artigo

`[O estudo contribui diretamente para a nossa pesquisa porque demonstra experimentalmente como a redução de dimensionalidade e a parada antecipada podem diminuir a quantidade de rodadas, o tempo de treinamento e o consumo de recursos no Aprendizado Federado. Além disso, utiliza imagens médicas e compara a abordagem proposta com o FedAvg tradicional, aproximando-se diretamente do contexto escolhido pelo grupo.]`

### Comentário crítico

`[O artigo apresenta alta relevância prática por avaliar Aprendizado Federado em um cenário médico multicêntrico e demonstrar reduções expressivas de tempo, rodadas e energia. Como fragilidades, utiliza o FedAvg clássico como principal linha de base, depende de PCA para redução dimensional e trabalha com uma aplicação clínica específica. Assim, seus resultados são promissores, mas devem ser generalizados com cautela.]`

### Citação literal opcional

> `["reduced the number of global training rounds from 200 to 38"]`

Página: `[1 do PDF]`
## Artigo 7 — Eshwarappa et al. (2025)
## Identificação do artigo

- Referência completa: `[ESHWARAPPA, Nithin Melala et al. Communication-efficient and privacy-preserving federated learning for medical image classification in multi-institutional edge computing. Journal of Cloud Computing, v. 14, art. 44, 2025.]`
- DOI ou URL: `[https://doi.org/10.1186/s13677-025-00734-z]`
- Base de origem: `[Google Scholar / SpringerLink]`
- Leitor responsável: `[Gabriel Anastácio Pereira]`
- Data da leitura: `[08/10/2026]`

## Fichamento

### Problema investigado

`[O estudo aborda a dificuldade do diagnóstico precoce e preciso do câncer de pele em ambientes médicos. Investiga a necessidade de preservar a privacidade dos dados de pacientes (o que inviabiliza o Aprendizado Centralizado - CL devido aos riscos de vazamento e alto consumo de banda) e os atrasos significativos de treinamento e comunicação provocados pelo Aprendizado Federado tradicional (FedAvg) ao lidar com a transferência contínua de parâmetros e com a escassez/heterogeneidade de dados locais.]`

### Objetivo do estudo

`[Propor, implementar e avaliar o método Edge-Average Federated Learning (Edge-Avg) em um ecossistema de computação em borda multi-institucional de duas camadas. O objetivo é otimizar o compromisso entre latência de comunicação e computação na classificação de imagens de lesões dermatológicas (benignas vs. malignas), alcançando alta precisão diagnóstica, menor tempo de treinamento e estrito cumprimento das normas de privacidade médica.]`

### Método utilizado

`[Arquitetura de Borda em Duas Camadas: Estruturada em um nível de Dispositivos IoT (captura) e um nível de Servidores de Borda locais (processamento e agregação intermediária) conectados a um Sistema de Informação Federado (FIS).Rede Neural e Aprendizado por Transferência: Utilização da arquitetura DenseNet121 pré-treinada no ImageNet89. Para viabilizar a execução eficiente na borda, os parâmetros treináveis do modelo foram reduzidos de 7.137.858 para apenas 100.354. Agregação na Borda (Edge-Avg): Diferente do FedAvg tradicional (que realiza a agregação apenas no servidor central/FIS), a agregação dos pesos locais ocorre diretamente nos servidores de borda das instituições antes do envio ao FIS.Modelagem Matemática da Latência: A latência total é formalizada como a soma da latência de comunicação, e da latência de computação, envolvendo o número de épocas e tempo de processamento por época.Aumento de Dados e Privacidade: Aplicação de rotação, escala, zoom, espelhamento e técnicas de privacidade diferencial para mitigar o overfitting e compensar limitações de dados locais.]`

### Contexto, amostra ou dados

`[Ambiente Experimental: Simulação em ambiente Google Colab Pro+ (GPU) com Python 3 e TensorFlow 2.13, configurado com 4 clientes distribuídos.ISIC-2019: 3.297 imagens dermatológicas (1.800 benignas e 1.497 malignas), redimensionadas para 224 X 224 pixels (80% treino, 20% validação).HAM10000 e ISIC-2020: Utilizados para validação cruzada do tempo global de treinamento e latência.]`


### Principais resultados

`[Redução da Latencia no Treinamento, ISIC-2019: Edge-Avg levou 3,14 min vs. 4,15 min do FedAvg (-24,33%) e 6,00 min do CL (-47,66%), HAM10000: Edge-Avg levou 9,53 min vs. 12,00 min do FedAvg (-20,58%) e 18,22 min do CL (-47,69%). ISIC-2020: Edge-Avg levou 29,54 min vs. 41,70 min do FedAvg (-29,16%) e 57,28 min do CL (-48,42%). Acurácia e Métricas de Desempenho (Taxa de aprendizado lr = 5 X 10⁴, FedAvg Tradicional: Alcançou acurácia máxima de 90,92% e menor taxa de perda de 0,38, Edge-Avg (Proposto): Superou o FedAvg ao atingir acurácia de 93,94%, loss de 0,370, e valores de 0,939 para Precisão, Revocação e F1-Score, superando o estado da arte na literatura recente.]`

### Limitações apresentadas

`[Sensibilidade a Hiperparâmetros: Demonstrou-se que o desempenho do FedAvg e do Edge-Avg cai consideravelmente fora do limiar ideal da taxa de aprendizado (ex.: caindo para 87,87% no FedAvg com lr = 5 X 10⁻³, evidenciando riscos de instabilidade ou overfitting. Dependência de Arquitetura de Borda: A redução do tempo de comunicação exige a presença de servidores de borda intermediários capazes de realizar agregação, o que nem todas as redes médicas descentralizadas possuem. Falta de Interpretabilidade: O modelo não inclui mecanismos de Inteligência Artificial Explicável (XAI), o que os próprios autores apontam como necessidade para adoção clínica real.]`

### Contribuição para o nosso artigo

`[Este estudo contribui diretamente para a nossa pesquisa sobre a Complexidade de Algoritmos em Aprendizado Federado, pois: Fornece a formalização matemática da latência no FedAvg (decompondo o tempo em componentes de comunicação de parâmetros e computação local).Serve como estudo de caso empírico sobre como o tamanho do modelo e a frequência de agregação impactam diretamente a complexidade temporal do FedAvg tradicional.Demonstra quantitativamente o impacto da taxa de aprendizado (lr = 5 X 10⁻⁴) na velocidade de convergência e na estabilidade do algoritmo em dados médicos distribuídos]`

### Comentário crítico

`[Pontos Fortes: Formalização clara das equações de latência. Redução inteligente do número de parâmetros do DenseNet121 de 7,1M para 100k. Validação rigorosa em múltiplos datasets públicos consolidados.Pontos Fracos / Fragilidades: A simulação foi limitada a 4 clientes em um ambiente controlado de GPU (Google Colab Pro+), o que simplifica os gargalos reais de redes com alta heterogeneidade de dispositivos e conectividade instável. O ganho de velocidade depende da inserção de uma camada extra de borda, o que altera a topologia padrão do FedAvg puro.]`

### Citação literal opcional

> `["The edge-average federated learning (Edge-Avg) method improved the training latency by 24% and 47% compared with the federated learning (Fed-Avg) and CL approaches, respectively... In terms of accuracy, our Edge-Avg approach surpassed the Fed-Avg method by achieving a better accuracy of 93.94% compared to the traditional method in the classification of skin cancer images into benign or malignant categories."]`

Página: `[Página: 1-2 (Abstract)]`

## Artigo 8 — Le et al. (2026)

## Identificação do artigo

- Referência completa: `[LE, Thu Thuy et al. Federated learning for medical image analysis: methods, challenges, and future directions. Advanced Engineering Informatics, v. 76, art. 104976, 2026.]`
- DOI ou URL: `[https://doi.org/10.1016/j.aei.2026.104976]`
- Base de origem: `[ScienceDirect / Google Scholar]`
- Leitor responsável: `[Matheus Soares]`
- Data da leitura: `[13/10/2026]`

## Fichamento

### Problema investigado

`[O estudo investiga os principais desafios que dificultam a aplicação ampla do Aprendizado Federado na análise de imagens médicas. Entre os problemas analisados estão a heterogeneidade dos dados entre instituições, distribuições não-IID, falta de dados rotulados, elevados custos de comunicação durante o treinamento, dificuldades na agregação dos modelos e riscos de privacidade e segurança associados às atualizações compartilhadas.]`

### Objetivo do estudo

`[O objetivo do artigo é apresentar uma revisão abrangente dos métodos, desafios e tendências recentes do Aprendizado Federado aplicado à análise de imagens médicas, considerando trabalhos publicados entre 2020 e 2025. O estudo busca identificar soluções desenvolvidas para os principais problemas da área e apontar direções futuras de pesquisa.]`

### Método utilizado

`[O trabalho realiza uma revisão da literatura sobre Aprendizado Federado aplicado à análise de imagens médicas. Os autores analisam estudos publicados entre 2020 e 2025 em periódicos e conferências relevantes e organizam a literatura em diferentes categorias de desafios, incluindo escassez de dados e rótulos, heterogeneidade e dados não-IID, custos de comunicação e agregação de modelos, além de privacidade e segurança.]`

### Contexto, amostra ou dados

`[O estudo está inserido no contexto da inteligência artificial aplicada à análise de imagens médicas, incluindo diferentes modalidades de imagem e aplicações clínicas. A revisão considera pesquisas em Aprendizado Federado publicadas entre 2020 e 2025 em periódicos e conferências das áreas de imagens médicas, inteligência artificial e aprendizado federado.]`

### Principais resultados

`[A revisão identificou que os principais desafios do Aprendizado Federado em imagens médicas estão relacionados à heterogeneidade dos dados, distribuições não-IID, falta de dados rotulados, custos de comunicação, agregação dos modelos e riscos de privacidade. O estudo também mostra que diferentes estratégias vêm sendo utilizadas para enfrentar essas dificuldades, incluindo aprendizado semissupervisionado e não supervisionado, técnicas para lidar com domain shift, modelos personalizados e arquiteturas avançadas de deep learning.]`

### Limitações apresentadas

`[Por se tratar de uma revisão focada em trabalhos publicados entre 2020 e 2025 e especificamente em análise de imagens médicas, o estudo não representa toda a literatura existente sobre Aprendizado Federado. Além disso, permanecem desafios em aberto relacionados à heterogeneidade dos dados, eficiência de comunicação, privacidade, personalização dos modelos e implantação do Aprendizado Federado em ambientes clínicos reais.]`

### Contribuição para o nosso artigo

`[Este estudo contribui diretamente para a nossa pesquisa ao apresentar uma visão atualizada dos principais desafios do Aprendizado Federado em imagens médicas, incluindo especificamente os custos de comunicação e a agregação dos modelos. A revisão ajuda a contextualizar como fatores como heterogeneidade dos dados, comunicação frequente e arquitetura dos modelos podem afetar a eficiência do treinamento federado, complementando os estudos específicos sobre FedAvg analisados pelo grupo.]`

### Comentário crítico

`[O principal ponto forte do artigo é reunir e organizar pesquisas recentes sobre Aprendizado Federado aplicado à análise de imagens médicas, permitindo identificar de forma clara os principais desafios e tendências da área. O estudo é especialmente útil por relacionar aspectos de comunicação, heterogeneidade, privacidade e técnicas de otimização. Como limitação, por ser uma revisão ampla, não aprofunda exclusivamente a complexidade computacional do FedAvg nem apresenta uma avaliação experimental própria sobre número de clientes, quantidade de rodadas ou tamanho do modelo. Dessa forma, sua contribuição para o nosso trabalho é principalmente contextual e comparativa.]`

### Citação literal opcional

> `["FL requires medical devices or facilities to continuously send local model updates to the central server"]`

Página: `[1 / Introduction]`


## Checklist

- [X] O artigo foi lido além do resumo.
- [X] O método e os resultados foram identificados.
- [X] As limitações foram registradas.
- [X] A conexão com o tema foi explicada.
- [X] Toda citação literal contém página.
