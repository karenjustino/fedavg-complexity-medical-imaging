# Etapa (a) — Escolha do Tema

> **Como preencher:** este documento deve ser preenchido **em conjunto pelo grupo**, mas com registro individualizado da contribuição de cada integrante. Substitua os campos entre `[ ]` pelas informações do seu grupo. Não apague as instruções em itálico — elas ajudam na avaliação do orientador.

---

## 1. Identificação do Grupo

| Campo | Informação |
|---|---|
| Curso / Disciplina | `[ Ciência da Computação — Computabilidade e Complexidade de Algoritmos]` |
| Projeto de Pesquisa / IC | `[Projeto de pesquisa Mostra de Tecnologia 2026.2]` |
| Orientador(a) | `[Profª Dorª Andréa Ono Sakai]` |
| Data de entrega desta etapa | `[dd/mm/aaaa]` |
| Integrantes do grupo | `[Gabriel Anastácio Pereira,Gabriel Alves Dias Reis, Karen Gabrielle Justino, Marcos Antonio da Silva Souza, Matheus Silva Soares]` |

---

## 2. Tema Escolhido

### 2.1 Área geral de interesse
*Qual grande área do conhecimento/disciplina motivou a escolha (ex.: complexidade dos algoritmos, classes de problemas P, NP, Algoritmos Gulosos, Programação Dinâmica, Divisão e conquista)?*

`[área geral de interesse é a Inteligência Artificial Distribuída (Aprendizado de Máquina) em interseção com a otimização de infraestrutura Cloud e Cibersegurança, analisada estritamente sob os tópicos de Complexidade de Algoritmos. O foco recai sobre a notação assintótica (O, Θ) aplicada à redução do custo computacional nos servidores Cloud durante os rounds de comunicação; na modelagem das ameaças bizantinas como classes de problemas P/NP/NP-Completo; e na aplicação de técnicas de Divisão e Conquista e Algoritmos Gulosos para orquestrar e otimizar a seleção de nós locais sem esgotar os recursos da nuvem.]`

### 2.2 Tema delimitado (versão final)
*Escreva o tema já delimitado, de forma específica — não o tema amplo. Lembre-se: o tema deve ser enunciado em 1 a 2 frases, como um assunto (ainda não é uma pergunta de pesquisa, isso vem na etapa "c").*

> **Tema:** `[Complexidade computacional e de comunicação do FedAvg em cenários simulados de Aprendizado Federado para classificação de imagens médicas.]`

### 2.3 Do amplo ao específico
*Mostre o raciocínio de delimitação — como vocês chegaram do tema amplo ao tema específico.*

| Tema amplo (ponto de partida) | Tema delimitado (ponto de chegada) |
|---|---|
| `[Inteligência Artificial aplicada à saúde]` | `[Aprendizado Federado para diagnóstico por imagens médicas]` |
| `[Aprendizado de Máquina distribuído]` | `[Segurança cibernética e privacidade em sistemas de Aprendizado Federado para imagens médicas]`|
| `[Complexidade de algoritmos distribuídos]` | `[Complexidade de comunicação e convergência de algoritmos de agregação (ex.: FedAvg) em cenários com múltiplos hospitais]`|
| `[Cloud Computing e segurança de dados]` | `[Uso de infraestrutura Cloud e aspectos de segurança e privacidade como contexto do treinamento federado]`|

---

## 3. Justificativa da Escolha

### 3.1 Relevância
*Por que esse tema é importante ou atual? Para quem ele importa (academia, mercado, sociedade)?*

`[O uso de Inteligência Artificial na área da saúde depende de grandes volumes de dados, porém informações médicas possuem caráter sensível e não podem ser compartilhadas livremente entre instituições. O Aprendizado Federado surge como uma alternativa que permite o treinamento colaborativo de modelos sem a necessidade de centralizar diretamente os dados dos participantes. Entretanto, essa abordagem apresenta desafios relacionados ao custo computacional, à quantidade de comunicação necessária entre clientes e servidor e à convergência do modelo.]`

### 3.2 Viabilidade
*O grupo avaliou se tem tempo, recursos, acesso a dados/fontes e domínio mínimo do assunto para desenvolver esse tema até o fim do projeto?*

| Critério | Avaliação (Sim/Parcial/Não) | Observação |
|---|---|---|
| Tempo disponível é suficiente | `[Sim]` | `[O cronograma do semestre é compatível com a carga de pesquisa teórica e a modelagem matemática assintótica exigida para a Mostra de Tecnologia, visto que o grupo adotou uma divisão estratégica de funções para otimizar o tempo e garantir as entregas de cada fase do projeto ]`|
| Há acesso a fontes/dados necessários | `[Sim]` | `[A fundamentação teórica será suportada por bases científicas de alto impacto (IEEE Xplore, ACM, PubMed, arXiv, PMC e DOAJ) e pelas documentações oficiais de arquitetura dos grandes provedores de Nuvem.]` |
| O grupo já tem domínio mínimo do tema | `[Parcial]` | `[Possuímos base sólida nas teorias de algoritmos e GRC (Governança, Riscos e Complice), porém será necessário aprofundamento prático em frameworks de simulação de Aprendizado Federado (como o Flower) e em arquitetura Cloud para simulação de possiveis comparaçãoes durante a pesquisa]` |
| Recursos técnicos necessários estão disponíveis | `[sim]` | `[A simulação das redes e a análise de complexidade dos nós podem ser executadas utilizando ambientes gratuitos ou de baixo custo na nuvem (ex.: Google Colab, AWS Free Tier) e os computadores pessoais do grupo.]` |

### 3.3 Originalidade / Não-redundância
*O grupo verificou rapidamente (via um levantamento preliminar) se o tema já é excessivamente explorado ou se existe um ângulo próprio a ser explorado?*

`[Apesar de existirem diversos estudos sobre Aprendizado Federado, o projeto busca analisar o FedAvg a partir da perspectiva da Complexidade de Algoritmos. O diferencial está em observar separadamente como parâmetros como número de clientes, quantidade de rodadas e tamanho do modelo podem influenciar o custo computacional, o custo de comunicação e a convergência do treinamento federado. A aplicação em cenários simulados de classificação de imagens médicas permite relacionar essa análise a um contexto real de uso da Inteligência Artificial, mantendo segurança, privacidade e infraestrutura Cloud como aspectos complementares da pesquisa.]`

---

## 4. Validação com o Orientador

| Campo | Informação |
|---|---|
| Data da conversa/validação | `[dd/mm/aaaa]` |
| Tema aprovado pelo orientador? | `[Sim / Sim com ajustes / Não]` |
| Observações ou ajustes solicitados pelo orientador | `[preencher]` |

---

## 5. Contribuição Individual dos Integrantes

> **Importante:** cada integrante deve descrever, com suas próprias palavras, o que efetivamente fez nesta etapa. Contribuições genéricas como "ajudei em tudo" não serão aceitas. Use verbos de ação e seja específico (ex.: "pesquisei 5 temas candidatos e apresentei prós/contras ao grupo").

### Integrante 1 — `[Gabriel Anastácio Pereira]`
- **O que fez nesta etapa:** `[Pesquisei possíveis aplicações de Inteligência Artificial na área da saúde e ajudei o grupo a definir o uso de Aprendizado Federado com imagens médicas como contexto da pesquisa. Também contribuí na discussão para deixar o tema mais relacionado aos conteúdos da disciplina.]`
- **Tempo dedicado (aprox.):** `[3h]`
- **Evidência da contribuição** *(print de conversa, rascunho, e-mail, documento compartilhado etc.)*: `[Participação na definição da aplicação do Aprendizado Federado em imagens médicas e na delimitação inicial do tema.]`

### Integrante 2 — `[Gabriel Alves Dias Reis]`
- **O que fez nesta etapa:** `[Entraram no grupo]`
- **Tempo dedicado (aprox.):** `[-------------]`
- **Evidência da contribuição:** `[-------------]`

### Integrante 3 — `[Karen Gabrielle Justino]`
- **O que fez nesta etapa:** `[Conduzi reuniões de alinhamento com o grupo e propus o tema central de IA Federada em Cloud cruzado com a disciplina. Além disso, estruturei as planilhas de controle bibliográfico e elaborei as strings de busca booleanas (em inglês e português) para as bases de dados, utilizando ferramentas de IA como o NotebookLM para auxílio na organização das fontes.]`
- **Tempo dedicado (aprox.):** `[5h Aprox]`
- **Evidência da contribuição:** `[Organização inicial do tema, estruturação dos materiais de pesquisa e definição das primeiras estratégias de busca bibliográfica.`

### Integrante 4 — `[Marcos Antonio da Silva Souza]`
- **O que fez nesta etapa:** `[Entraram no grupo]`
- **Tempo dedicado (aprox.):** `[-------------]`
- **Evidência da contribuição:** `[-------------]`

### Integrante 5 — `[Matheus Silva Soares]`
- **O que fez nesta etapa:** `[Ajudei a relacionar o tema de Aprendizado Federado com Complexidade de Algoritmos e Cibersegurança. Pesquisei possibilidades para delimitar o assunto e contribuí para definir que o projeto deveria analisar o FedAvg, considerando principalmente o custo computacional, a comunicação entre clientes e servidor e a proteção dos dados médicos.]`
- **Tempo dedicado (aprox.):** `[3h]`
- **Evidência da contribuição:** `[Participação na delimitação do tema e na definição da relação entre FedAvg, complexidade, segurança e dados médicos.]`

*(Copie o bloco acima para cada integrante adicional do grupo.)*

### 5.1 Quadro-resumo de participação

| Integrante | Contribuição principal | % estimado de participação nesta etapa |
|---|---|---|
| `[Gabriel Anastácio Pereira]` | `[Pesquisa sobre IA, Aprendizado Federado e imagens médicas]` | `[25%]` |
| `[Gabriel Alves Dias Reis]` | `[Entrou no grupo após esta etapa]` | `[0%]` |
| `[Karen Gabrielle Justino]` | `[Organização do tema e estruturação inicial da pesquisa]` | `[40%]` |
| `[Marcos Antonio da Silva Souza]` | `[Entrou no grupo após esta etapa]` | `[0%]` |
| `[Matheus Silva Soares]` | `[Delimitação do tema entre FedAvg, complexidade e segurança]` | `[35%]` |

*A soma das porcentagens deve ser igual a 100%. Divergências de percepção sobre a participação devem ser discutidas em grupo antes do envio — o orientador pode solicitar esclarecimentos individuais em caso de disparidade relevante.*

---

## 6. Checklist Final da Etapa

- [x] Tema delimitado e redigido em 1-2 frases
- [x] Justificativa de relevância escrita
- [x] Viabilidade avaliada pelo grupo
- [x] Verificação preliminar de originalidade realizada
- [x] Tema validado com o orientador
- [x] Contribuição individual de cada integrante registrada
- [x] Quadro-resumo de participação preenchido (soma = 100%)

---


