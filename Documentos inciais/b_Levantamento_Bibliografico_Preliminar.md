# Etapa (b) — Levantamento Bibliográfico

> **Como preencher:** este documento deve ser preenchido **em conjunto pelo grupo**, mas com registro individualizado da contribuição de cada integrante em cada passo. Substitua os campos entre `[ ]` pelas informações do seu grupo. Não apague as instruções em itálico — elas ajudam na avaliação do orientador.

---

## 1. Identificação do Grupo

| Campo | Informação |
|---|---|
| Curso / Disciplina | `[Ciência da Computação — Computabilidade e Complexidade de Algoritmos]` |
| Projeto de Pesquisa / IC | `[Projeto de pesquisa Mostra de Tecnologia 2026.2]` |
| Orientador(a) | `[Profª Dorª Andréa Ono Sakai]` |
| Data de entrega desta etapa | `[dd/mm/aaaa]` |
| Integrantes do grupo | `[Gabriel Anastácio Pereira,Gabriel Alves Dias Reis, Karen Gabrielle Justino, Marcos Antonio da Silva Souza, Matheus Silva Soares]` |
| Tema (da etapa "a") | `[Complexidade computacional e de comunicação do FedAvg em cenarios simulados de apredindizado federado para classificação de imagens médicas]` |

---

## FASE 1 — Planejamento da Busca

### Passo 1 — Pergunta de pesquisa e palavras-chave

**1.1 Problema/pergunta de pesquisa (versão de trabalho)**
*Ainda não precisa ser a versão final (isso vem na etapa "c"), mas deve orientar a busca desta fase.*

> `[Como números de clientes, a quantidade de rodadas e o tamanho do modelo afetam os custos computacional e de comunicação do FedAvg em um ambiente simulado? ]`

**1.2 Conceitos-chave e sinônimos**
*Liste os conceitos centrais da pergunta e seus sinônimos, em português e inglês.*

| Conceito-chave | Sinônimos / termos relacionados (PT) | Sinônimos / termos relacionados (EN) |
|---|---|---|
| `[Aprendizado Federado]` | `[aprendizado distribuído, aprendizado colaborativo]` | `[federated learning, distributed learning, collaborative learning]` |
| `[Segurança e privacidade]` | `[proteção de dados, privacidade diferencial, vulnerabilidade]` | `[security, privacy, differential privacy, vulnerability]` |
| `[Imagens médicas]` | `[diagnóstico por imagem, mamografia, radiologia ]` | `[medical imaging, mammography, radiology, healthcare]` |

*Responsável por este passo: `[Karen Gabrielle Justino]`*

---

### Passo 2 — Strings de busca

*Combine os termos do passo 1 com operadores booleanos (`AND`, `OR`, `NOT`). Use aspas para termos compostos e truncamento (`*`) quando a base permitir.*

| Nº | String de busca | Base(s) em que será usada | Elaborada por |
|---|---|---|---|
| 1 | `[("Federated Learning" OR "FedAvg" OR "Federated Averaging") AND ("Number of Clients" OR "Rounds" OR "Model Size") AND ("Computational Complexity" OR "Communication Cost" OR "Overhead")]` | `[PUBMED / IEEE / ScienceDirect ]` | `[Karen Justino]` |
| 2 | `[("federated learning" OR "FedAvg) AND ("Complexity" OR "Algorithm") ("security" OR "LGPD") ]` | `[Google scholar / PUBMED / IEEE / sciencedirect ]` | `[Matheus Soares]` |
| 3 | `[( "Federal Learning" OR "FedAvg ) AND ( cloud ) AND ( Security OR Privacy)]` | `[ IEEE  ]` | `[Marcos Antonio]` |
| 4 | `[("artificial intelligence" OR "machine learning") AND ("federated learning") AND ("medical imaging")]` | `[ IEEE Xplore, PubMed, Google Scholar ]` | `[Gabriel Anastácio]` |
| 5 | `[("Federated Learning" OR "FedAvg) AND ("Complexity") AND ("Algorithm")]` | `[  IEEE Xplore, PubMed, Google Scholar  ]` | `[Gabriel Alves]` |

---

### Passo 3 — Bases de dados escolhidas

*Selecione de 2 a 4 bases relevantes ao tema. Registre a justificativa — isso vai para a seção de metodologia do artigo/relatório de IC.*

| Base de dados | Por que foi escolhida | Responsável pela busca nesta base |
|---|---|---|
| `[ PubMed / PMC]` | `[Artigos focado em pesquisa médica com o uso ]` | `[Karen Justino / Gabriel Anastácio / Gabriel Alves / Matheus Soares]` |
| `[ IEEE Xplore]` | `[ Possui estudos técnicos sobre IA, cibersegurança e computação. ]` | `[Karen Justino / Matheus Soares / Marcos Antonio / Gabriel Anastácio / Gabriel Alves]]` |
| `[ ScienceDirect ]` | `[ Reúne artigos de tecnologia, saúde e segurança. ]` | `[Karen Justino / Matheus Soares]` |
| `[ Google Scholar ]` | `[ Facilita a busca por diferentes tipos de trabalhos acadêmicos. ]` | `[Matheus Soares / Gabriel Anastácio / Gabriel Alves]` |

---

### Passo 4 — Critérios de inclusão e exclusão

**Critérios de inclusão:**
- `[Artigos publicados nos últimos 10 anos]`
- `[Revisados por pares]`
- `[Em português/inglês]`
- `[Disponíveis na íntegra]`

**Critérios de exclusão:**
- `[Resumos sem texto completo, duplicatas ou artigos não revisados por pares ]`
- `[Artigos com sobreposição direta ao objetivo algoritmo dos grupos]`
- `[Estudos que classificam ameaças bizantinas com P/NP ou que afirmem NP_Completude sem formulação matemática e prova]`
- `[Trabalhos que abordem a privacidade de dados como uma garantia absoluta, em vez de focar na redução de risco]`

*Definidos em conjunto por: `[Gabriel Anastácio Pereira, Gabriel Alves Dias Reis, Karen Gabrielle Justino, Marcos Antonio da Silva Souza, Matheus Silva Soares]`*

---

## FASE 2 — Execução da Busca e Triagem

### Passo 5 — Execução das buscas e registro dos resultados

*Anote quantos resultados cada string trouxe em cada base (útil para o fluxograma tipo PRISMA, se o projeto exigir). Exporte as referências (BibTeX, RIS, CSV) para um gerenciador de referências.*

| Base | String usada (nº) | Data da busca | Nº de resultados | Executada por |
|---|---|---|---|---|
| `[ Google scholar / PUBMED / IEEE / sciencedirect ]` | `[("federated learning" OR "FedAvg") AND ("Complexity" OR "Algorithm") ("security" OR "LGPD") ]` | `[31/08/2026]` `[07/09/2026]` | `[14]` | `[Matheus Soares]` |
| `[PubMed / IEEE Xplore / ScienceDirect ]` | `[("FedAvg" OR "Federated Averaging") AND "Computational Complexity" AND "Communication Complexity" NOT ("Byzantine" OR "NP-Complete" OR "NP-Hard") ]` | `[03/09/2026]` | `[07/09/2026 ]` | `[14]` | `[Karen Justino]` |
| `[IEEE Xplore ]` | `[("Federated Learning" OR "FedAvg") AND ("cloud") AND ("Security" OR "Privacy") ]` | `[dd/mm/aaaa]` |  `[04/09/26]` `[07/09/2026 ]` | `[1]` | `[Marcos Antonio]` |
| `[IEEE Xplore / PubMed / Google Scholar ]` | `[("artificial intelligence" OR "machine learning") AND ("federated learning" OR "FedAvg") AND ("medical imaging") ]` |  `[05/09/26]` `[07/09/2026 ]` | `[13]` | `[Gabriel Anastácio]` |
| `[IEEE Xplore / PubMed / Google Scholar ]` | `[("Federated Learning" OR "FedAvg") AND ("Complexity") AND ("Algorithm") ]` | `[01/09/26]` `[07/09/2026 ]` | `[2]` | `[Gabriel Alves]` |

**Total de resultados brutos (soma de todas as buscas):** `[44]`

**Gerenciador de referências utilizado:** `[Zotero]`
**Formato de exportação:** `[BibTeX / RIS]`

---

### Passo 6 — Triagem por título e resumo (1ª filtragem)

*Leia apenas título e resumo de cada resultado. Classifique: incluir / excluir / dúvida. Remova duplicatas entre bases.*

| Item de controle | Quantidade |
|---|---|
| Total de resultados antes da triagem | `[44]` |
| Duplicatas removidas | `[3]` |
| Classificados como "Incluir" | `[9]` |
| Classificados como "Excluir" | `[11]` |
| Classificados como "Dúvida" | `[21]` |

*A triagem detalhada, artigo por artigo, deve ser registrada na planilha de controle do projeto (aba "Triagem de Artigos"). Aqui, registre apenas o resumo quantitativo.*

**Como as dúvidas foram resolvidas?** *(ex.: discussão em grupo, consulta ao orientador)*
`[As dúvidas foram resolvidas após a leitura da introdução e da conclusão dos artigos, seguida de discussão em grupo e comparação com os critérios de inclusão e exclusão. Ao final, os artigos foram reclassificados como “Incluir” ou “Excluir”.]`

*Responsável(is) por esta triagem: `[Gabriel Alves Dias Reis, Karen Gabrielle Justino, Matheus Silva Soares]`*

---

### Passo 7 — Triagem por leitura completa (2ª filtragem)

*Para os artigos que passaram na primeira filtragem, leia introdução e conclusão. Aplique os critérios de inclusão/exclusão (passo 4) de forma mais rigorosa.*

| Item de controle | Quantidade |
|---|---|
| Total de artigos que entraram nesta filtragem | `[30]` |
| Aprovados (conjunto definitivo para fichamento) | `[20]` |
| Excluídos nesta etapa | `[10]` |

**Principais motivos de exclusão nesta filtragem:**
- `[O artigo foi excluído por apresentar relação apenas indireta com o Aprendizado Federado, sem contribuir de forma significativa para os principais eixos da pesquisa: complexidade algorítmica, computação em nuvem, cibersegurança, privacidade ou imagens médicas. ]`
- `[O artigo foi excluído por não apresentar análise suficiente sobre custo computacional, comunicação entre clientes e servidor, convergência, segurança, privacidade ou aplicação médica, não contribuindo diretamente para os objetivos definidos no estudo. ]`

*Responsável(is) por esta triagem: `[Gabriel Anastácio Pereira, Gabriel Alves Dias Reis, Karen Gabrielle Justino, Matheus Silva Soares]`*

---

## 3. Lista Final de Artigos Selecionados (Conjunto Definitivo)

*Liste aqui os artigos que passaram por todas as filtragens e seguirão para o fichamento (etapa "j"). Referência completa no formato ABNT/APA definido pelo projeto.*

1. `[NANAKARAN, Negin Piran; UKWATTA, Eranga. A novel federated learning framework for medical imaging: resource-efficient approach combining PCA with early stopping. Medical Physics, v. 52, n. 8, e18064, 2025. DOI: 10.1002/mp.18064. Disponível em: https://pmc.ncbi.nlm.nih.gov/articles/PMC12409104/. Acesso em: 7 set. 2026.]`
2. `[MCMAHAN, H. Brendan; MOORE, Eider; RAMAGE, Daniel; HAMPSON, Seth; AGUERA Y ARCAS, Blaise. Communication-efficient learning of deep networks from decentralized data. Proceedings of the 20th International Conference on Artificial Intelligence and Statistics, v. 54, p. 1273–1282, 2017. Disponível em: https://proceedings.mlr.press/v54/mcmahan17a.html.]`
3. `[LI, Xiang; HUANG, Kaixuan; YANG, Wenhao; WANG, Shusen; ZHANG, Zhihua. On the convergence of FedAvg on non-IID data. International Conference on Learning Representations – ICLR, 2020. Disponível em: https://arxiv.org/abs/1907.02189.]`
4. `[CHENG, Yifei et al. Communication-efficient federated learning with stagewise training strategy. Neural Networks, v. 167, p. 460–472, 2023. DOI: 10.1016/j.neunet.2023.08.033. Disponível em: https://www.sciencedirect.com/science/article/pii/S0893608023004549.]`
5. `[GAO, Hongchang; XU, An; HUANG, Heng. On the convergence of communication-efficient Local SGD for Federated Learning. Proceedings of the AAAI Conference on Artificial Intelligence, v. 35, n. 9, p. 7510–7518, 2021. DOI: 10.1609/aaai.v35i9.16920. Disponível em: https://ojs.aaai.org/index.php/AAAI/article/view/16920.]`
6. `[LE, Thu Thuy et al. Federated learning for medical image analysis: methods, challenges, and future directions. Advanced Engineering Informatics, v. 76, art. 104976, 2026. DOI: 10.1016/j.aei.2026.104976. Disponível em: https://www.sciencedirect.com/science/article/pii/S1474034626006683.]`
7. `[SANDHU, Sukhveer Singh et al. Medical Imaging Applications of Federated Learning. Diagnostics, v. 13, n. 19, art. 3140, 2023. DOI: 10.3390/diagnostics13193140. Disponível em: https://www.mdpi.com/2075-4418/13/19/3140.]`
8. `[FANG, Chen; GUO, Yuanbo; WANG, Na; JU, Ankang. Highly efficient federated learning with strong privacy preservation in cloud computing. Computers & Security, v. 96, art. 101889, 2020. DOI: 10.1016/j.cose.2020.101889. Disponível em: https://www.sciencedirect.com/science/article/abs/pii/S0167404820301620.]`
9. `[KOUTSOUBIS, Nikolas et al. Privacy-preserving Federated Learning and Uncertainty Quantification in Medical Imaging. Radiology: Artificial Intelligence, v. 7, n. 4, e240637, 2025. DOI: 10.1148/ryai.240637. Disponível em: https://pmc.ncbi.nlm.nih.gov/articles/PMC12319697/.]`
10. `[ALVARENGA, Luana F. et al. Legal and Ethical Considerations for Translating Federated Learning into Cross-Border Healthcare Innovation. IEEE Journal of Biomedical and Health Informatics, 2026. DOI: 10.1109/JBHI.2026.3677593. Disponível em: https://pubmed.ncbi.nlm.nih.gov/41880260/. Acesso em: 7 set. 2026.]`
11. `[KUMAR, K. A. Sathish; NELSON, Leema; JIBINSINGH, Betshrine Rachel. Systematic review of privacy-preserving Federated Learning in decentralized healthcare systems. Franklin Open, v. 13, art. 100440, 2025. DOI: 10.1016/j.fraope.2025.100440. Disponível em: https://www.sciencedirect.com/science/article/pii/S2773186325002257.]`
12. `[GHOSH, Durjoy et al. Advancements and challenges of federated learning in medical imaging: a systematic literature review. Artificial Intelligence Review, v. 59, art. 87, 2026. DOI: 10.1007/s10462-025-11489-z. Disponível em: https://link.springer.com/article/10.1007/s10462-025-11489-z.]`
13. `[ESHWARAPPA, Nithin Melala et al. Communication-efficient and privacy-preserving federated learning for medical image classification in multi-institutional edge computing. Journal of Cloud Computing, v. 14, art. 44, 2025. DOI: 10.1186/s13677-025-00734-z. Disponível em: https://link.springer.com/article/10.1186/s13677-025-00734-z.]`
14. `[XIA, Geming; CHEN, Jian; YU, Chaodong; MA, Jun. Poisoning Attacks in Federated Learning: A Survey. IEEE Access, v. 11, p. 10708–10722, 2023. DOI: 10.1109/ACCESS.2023.3238823. Disponível em: https://doi.org/10.1109/ACCESS.2023.3238823.]`
15. `[LI, Zhaozheng; LAN, Jiahe; YAN, Zheng; GELENBE, Erol. Backdoor attacks and defense mechanisms in federated learning: a survey. Information Fusion, v. 123, art. 103248, 2025. Disponível em: https://www.sciencedirect.com/science/article/pii/S1566253525003215.]`
16. `[STALLINGS, William; BROWN, Lawrie. Computer Security: Principles and Practice. 4. ed. Pearson, 2018. Disponível em: https://www.pearson.com/en-us/subject-catalog/p/computer-security-principles-and-practice/P200000003493.]`
17. `[BELOGLAZOV, Anton; ABAWAJY, Jemal; BUYYA, Rajkumar. Energy-aware resource allocation heuristics for efficient management of data centers for Cloud computing. Future Generation Computer Systems, v. 28, n. 5, p. 755–768, 2012. DOI: 10.1016/j.future.2011.04.017. Disponível em: https://www.sciencedirect.com/science/article/pii/S0167739X11000689.]`
18. `[IEEE. IEEE 3652.1-2020: IEEE Guide for Architectural Framework and Application of Federated Machine Learning. IEEE Standards Association, 2020. Disponível em: https://standards.ieee.org/ieee/3652.1/7453/.]`
19. `[MIR, Bilal Ahmad; ABBAS, Syed Raza; LEE, Seung Won. Federated Learning in Healthcare Ethics: A Systematic Review of Privacy-Preserving and Equitable Medical AI. Healthcare, v. 14, n. 3, art. 306, 2026. DOI: 10.3390/healthcare14030306. Disponível em: https://pmc.ncbi.nlm.nih.gov/articles/PMC12896918/.]`
20. `[KOGUT-CZARKOWSKA, Magdalena; SHABANI, Mahsa. Anonymization, accountability, and access: legal dimensions of health data sharing in federated networks. Perspectives from empirical study. Frontiers in Digital Health, v. 8, art. 1719728, 2026. DOI: 10.3389/fdgth.2026.1719728. Disponível em: https://www.frontiersin.org/journals/digital-health/articles/10.3389/fdgth.2026.1719728/full.]`

*(Adicione quantas linhas forem necessárias.)*

---

## 4. Contribuição Individual dos Integrantes

> **Importante:** cada integrante deve descrever, com suas próprias palavras, o que efetivamente fez em cada passo desta etapa. Contribuições genéricas como "ajudei em tudo" não serão aceitas. Use verbos de ação e seja específico (ex.: "executei a busca no IEEE Xplore com a string 2 e obtive 84 resultados; fiz a triagem por título/resumo de 40 desses").

### Integrante 1 — `[Gabriel Anastácio Pereira]`
- **Passo(s) em que atuou:** `[Passos 2, 3, 4, 5, 6 e 7]`
- **O que fez em cada passo:** `[Fiquei responsável por buscar artigos ligados à Inteligência Artificial, Aprendizado Federado e imagens médicas. Usei o IEEE Xplore, PubMed e Google Scholar e encontrei 13 trabalhos relacionados ao tema. Depois, ajudei a revisar os artigos que passaram para a leitura mais completa, observando principalmente a aplicação do Federated Learning na área médica.]`
- **Tempo dedicado (aprox.):** `[4h]`
- **Evidência da contribuição** *(print de busca, planilha de triagem, exportação BibTeX, etc.)*: `[Participação na pesquisa e seleção de artigos relacionados à Inteligência Artificial, Aprendizado Federado e imagens médicas.]`

### Integrante 2 — `[Gabriel Alves Dias Reis]`
- **Passo(s) em que atuou:** `[Passos 2, 3, 4, 5, 6 e 7]`
- **O que fez em cada passo:** `[Trabalhei mais na parte de algoritmos e complexidade do FedAvg. Pesquisei no IEEE Xplore, PubMed e Google Scholar e encontrei 2 artigos que ajudaram nessa parte do projeto. Também ajudei a separar os trabalhos mais úteis durante a triagem por título, resumo, introdução e conclusão.]`
- **Tempo dedicado (aprox.):** `[3h]`
- **Evidência da contribuição:** `[Contribuição na pesquisa e análise de artigos relacionados a FedAvg, algoritmos e complexidade.]`

### Integrante 3 — `[Karen Gabrielle Justino]`
- **Passo(s) em que atuou:** `[Passos 1, 2, 3, 4, 5, 6 e 7]`
- **O que fez em cada passo:** `[Ajudei a organizar a pergunta inicial da pesquisa e as palavras-chave usadas pelo grupo. Minha busca ficou mais voltada para número de clientes, rodadas, tamanho do modelo e custo computacional e de comunicação do FedAvg. Pesquisei no PubMed, IEEE Xplore e ScienceDirect, encontrando 14 artigos, e também participei das etapas de seleção e revisão dos trabalhos.]`
- **Tempo dedicado (aprox.):** `[6h]`
- **Evidência da contribuição:** `[Organização da pergunta de pesquisa, palavras-chave, buscas bibliográficas e apoio na seleção dos artigos.]`

### Integrante 4 — `[Marcos Antonio da Silva Souza]`
- **Passo(s) em que atuou:** `[Passos 2, 3, 4 e 5]`
- **O que fez em cada passo:** `[[Fiquei com a pesquisa mais voltada para Cloud Computing, segurança e privacidade no Aprendizado Federado. Fiz a busca no IEEE Xplore e selecionei um artigo que ajudou a complementar essa parte do trabalho, principalmente na relação entre nuvem e segurança.]`
- **Tempo dedicado (aprox.):** `[2h]`
- **Evidência da contribuição:** `[Pesquisa de conteúdos relacionados a Cloud Computing, segurança e privacidade no contexto do Aprendizado Federado.]`

### Integrante 5 — `[Matheus Silva Soares]`
- **Passo(s) em que atuou:** `[Passos 2, 3, 4, 5, 6 e 7]`
- **O que fez em cada passo:** `[Minha pesquisa ficou mais concentrada na ligação entre complexidade, FedAvg, segurança, LGPD e Cloud Computing. Busquei artigos no Google Scholar, PubMed, IEEE Xplore e ScienceDirect e encontrei 14 resultados. Também ajudei na triagem, comparando os artigos com o tema do projeto e verificando quais realmente contribuíam para complexidade, privacidade e imagens médicas.]`
- **Tempo dedicado (aprox.):** `[6h]`
- **Evidência da contribuição:** `[Pesquisa e análise de artigos sobre complexidade, segurança, LGPD, Cloud Computing e aplicações médicas do Aprendizado Federado.]`

*(Copie o bloco acima para cada integrante adicional do grupo.)*

### 4.1 Quadro-resumo de participação por passo

| Passo | Responsável(is) | % estimado de participação de cada um |
|---|---|---|
| 1. Pergunta e palavras-chave | `[Karen Gabrielle Justino]` | `[Karen: 100%]` |
| 2. Strings de busca | `[Gabriel Anastácio Pereira, Gabriel Alves Dias Reis, Karen Gabrielle Justino, Marcos Antonio da Silva Souza, Matheus Silva Soares]` | `[20% cada]` |
| 3. Bases de dados | `[Karen: 25%; Matheus: 25%; Gabriel Anastácio: 20%; Gabriel Alves: 20%; Marcos: 10%]` |
| 4. Critérios de inclusão/exclusão | `[Todos os integrantes]` | `[20% cada]` |
| 5. Execução das buscas |  `[Todos os integrantes]` | `[Karen: 32%; Matheus: 32%; Gabriel Anastácio: 29%; Gabriel Alves: 5%; Marcos: 2%]` |
| 6. Triagem título/resumo |  `[Gabriel Alves Dias Reis, Karen Gabrielle Justino, Matheus Silva Soares]` | `[Karen: 40%; Matheus: 40%; Gabriel Alves: 20%]` |
| 7. Triagem texto completo | `[Gabriel Anastácio Pereira, Gabriel Alves Dias Reis, Karen Gabrielle Justino, Matheus Silva Soares]` | `[Karen: 30%; Matheus: 30%; Gabriel Anastácio: 25%; Gabriel Alves: 15%]` |

### 4.2 Quadro-resumo geral de participação na etapa

| Integrante | % estimado de participação total nesta etapa |
|---|---|
| `[Gabriel Anastácio Pereira]` | `[20%]` |
| `[Gabriel Alves Dias Reis]` | `[15%]` |
| `[Karen Gabrielle Justino]` | `[30%]]` |
| `[Marcos Antonio da Silva Souza]` | `[10%]]` |
| `[Matheus Silva Soares]` | `[25%]` |

*A soma das porcentagens deve ser igual a 100%. Divergências de percepção sobre a participação devem ser discutidas em grupo antes do envio — o orientador pode solicitar esclarecimentos individuais em caso de disparidade relevante.*

---

## 5. Checklist Final da Etapa

**Fase 1 — Planejamento**
- [X] Pergunta de pesquisa de trabalho definida
- [X] Conceitos-chave e sinônimos (PT/EN) listados
- [X] Strings de busca elaboradas com operadores booleanos
- [X] Bases de dados escolhidas e justificadas
- [X] Critérios de inclusão e exclusão definidos

**Fase 2 — Execução e triagem**
- [X] Buscas executadas e resultados registrados por base/string
- [X] Referências exportadas para o gerenciador de referências
- [X] Triagem por título/resumo concluída (com duplicatas removidas)
- [X] Triagem por texto completo (introdução/conclusão) concluída
- [X] Conjunto definitivo de artigos para fichamento compilado

**Documentação**
- [X] Contribuição individual de cada integrante registrada por passo
- [X] Quadro-resumo de participação preenchido (soma = 100%)

---


