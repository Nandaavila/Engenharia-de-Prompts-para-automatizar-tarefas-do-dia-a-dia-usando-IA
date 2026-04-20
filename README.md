# Engenharia-de-Prompts-para-automatizar-tarefas-do-dia-a-dia-usando-IA
Projeto sobre Engenharia de Prompts para automação de tarefas do dia a dia usando Inteligência Artificial.

## 📌 Contexto

Com o avanço da Inteligência Artificial Generativa, a Engenharia de Prompts tornou-se uma habilidade essencial para comunicação eficiente entre humanos e modelos de linguagem (LLMs).

Este projeto foi desenvolvido com o apoio do NotebookLM, utilizando fontes confiáveis e práticas reais para demonstrar como prompts podem ser utilizados para automatizar tarefas do dia a dia e aumentar a produtividade.

---

## 🎯 Objetivos

Este projeto tem como principais objetivos:

- Compreender os fundamentos da Engenharia de Prompts
- Aplicar técnicas modernas de prompting
- Criar prompts reutilizáveis
- Automatizar tarefas do cotidiano
- Documentar testes e melhorias
- Desenvolver um MiniGuia prático reutilizável

---

## 📚 Curadoria de Fontes

As seguintes fontes foram utilizadas para o desenvolvimento deste projeto:

- GUIA PRÁTICO DE ENGENHARIA DE PROMPT 2024 por ROBINSON FELIX
 chrome-extension://efaidnbmnnnibpcajpcglclefindmkaj/https://reuellopes.com.br/wp-content/uploads/2024/09/ebook-prompts.pdf

- APOSTILA Engenharia de Prompts - TCESP.pdf
 chrome-extension://efaidnbmnnnibpcajpcglclefindmkaj/https://www.tce.sp.gov.br/sites/default/files/2024-11/Engenharia%20de%20prompts.pdf

- Microsoft – Prompt Engineering  
https://learn.microsoft.com/en-us/azure/ai-services/openai/concepts/prompt-engineering

- GUIA PRÁTICO ENGENHARIA DE PROMPT
chrome-extension://efaidnbmnnnibpcajpcglclefindmkaj/https://inova.coop.br/arquivos/Ensina/Guia_pr%C3%A1tico_InovaCoop_-_Engenharia_de_Prompt.pdf

- Engenharia de prompts: como aplicar no dia a dia
https://www.serasaexperian.com.br/conteudos/como-aplicar-engenharia-de-prompts/

---

## 🧪 Engenharia de Prompts e Cicatrizes

Durante o uso do NotebookLM, foram realizados testes sucessivos para melhorar a qualidade das respostas.

Abaixo estão os principais prompts utilizados e suas melhorias.

### Prompt Inicial

## Crie um guia completo sobre Engenharia de Prompt e o funcionamento dos modelos de linguagem (LLMs), incluindo fundamentos, técnicas e exemplos práticos.

## Resultado: O conteúdo estava extenso, mas sem organização clara para uso didático. Observe abaixo:

Como engenheiro de prompt, estruturei este guia completo para você dominar a comunicação com a Inteligência Artificial, compreendendo desde a arquitetura da máquina até a aplicação de comandos avançados na prática.

### 1. O Funcionamento dos Modelos de Linguagem (LLMs)
Para extrair o melhor de uma IA, é preciso primeiro entender como ela "pensa". Os Grandes Modelos de Linguagem (LLMs), como GPT-4, Claude e Gemini, são algoritmos de aprendizado profundo baseados na **arquitetura Transformer**. 

*   **Previsão de Tokens:** Os LLMs não "entendem" o texto de forma consciente. Eles operam de forma probabilística, calculando e prevendo qual é a próxima palavra (ou "token") mais provável em uma sequência, com base em bilhões de dados de treinamento.
*   **Mecanismo de Atenção (Self-Attention):** A arquitetura Transformer permite que o modelo avalie o peso e a importância de cada palavra do seu prompt em relação a todas as outras. Isso significa que a IA consegue analisar o contexto global da sua instrução, conectando palavras distantes para gerar respostas coerentes.
*   **Janela de Contexto (Context Window):** É o limite de "memória de curto prazo" da IA durante uma conversa. Tudo o que ultrapassa a janela de contexto (medida em tokens) é "esquecido" pelo modelo. Por isso, para tarefas muito longas, o contexto vital deve ser reafirmado.

### 2. Fundamentos da Engenharia de Prompt
A engenharia de prompt é a ciência empírica de planejar, criar, testar e refinar instruções para guiar a IA a gerar as saídas desejadas, minimizando erros e alucinações.

*   **A Regra de Ouro:** Formule suas instruções da mesma maneira detalhada e clara que faria ao delegar uma tarefa a um ser humano. Se o comando for ambíguo para uma pessoa, também será para a máquina.
*   **Frameworks de Estruturação:** Utilizar frameworks garante que nenhuma informação fique de fora:
    *   **P.R.O.M.P.T.:** Define a **P**ersona, o **R**oteiro, o **O**bjetivo, o **M**odelo de Saída, o **P**anorama (contexto) e a capacidade de **T**ransformar (iterar).
    *   **Matriz PACIF:** Estrutura o comando delimitando o **P**apel, a **A**ção, o **C**ontexto, a **I**ntenção e o **F**ormato final.

### 3. Técnicas de Prompting: Do Básico ao Avançado
Para controlar a "mente" probabilística dos LLMs, aplicamos técnicas que calibram o comportamento e o raciocínio da ferramenta:

*   **Zero-Shot e Few-Shot Prompting:**
    *   *Zero-Shot:* É a instrução direta, sem fornecer exemplos. Ideal para tarefas nas quais o modelo já possui alto conhecimento (ex: "Traduza esta frase para o francês").
    *   *Few-Shot:* Consiste em fornecer exemplos práticos de como a entrada e a saída devem se parecer dentro do próprio prompt. A IA reconhece o padrão linguístico e estrutural dos exemplos e o replica, aumentando drasticamente a precisão da resposta.
*   **Atribuição de Persona (Role Prompting):** Instruir o modelo a assumir um papel específico (ex: "Aja como um consultor financeiro sênior"). Isso altera imediatamente o tom de voz, a profundidade, a formalidade e o vocabulário da resposta.
*   **Cadeia de Pensamento (Chain of Thought - CoT):** Técnica essencial para matemática e problemas lógicos. Ao forçar a IA a "pensar passo a passo" ou ao demonstrar as etapas de raciocínio no prompt, você evita que o modelo tente adivinhar a resposta final imediatamente, reduzindo os erros de lógica.
*   **Restrições Negativas (O que NÃO fazer):** Delimite o comportamento da IA estabelecendo regras rígidas de exclusão (ex: "Não mencione os custos de instalação", "Evite jargões técnicos", "Não ultrapasse três parágrafos"). Isso mantém o modelo focado e previne "alucinações" ou divagações.
*   **Decomposição de Tarefas (Task Decomposition):** Para projetos extensos (como escrever um relatório de 20 páginas), não use um único prompt gigante. Divida o problema em subtarefas sequenciais (ex: primeiro gerar o esboço, depois a introdução, depois a análise), onde o resultado de uma etapa alimenta o prompt da próxima.
*   **Refinamento Iterativo:** Trate a IA como um parceiro de diálogo. Analise a resposta criticamente e envie novos prompts corrigindo as falhas do modelo, adicionando novas restrições ou pedindo que ele expanda detalhes específicos.

### 4. Exemplos Práticos de Aplicação
Abaixo, mostro como a combinação dessas técnicas funciona em cenários reais:

**A. Resumo Estruturado de Textos Longos**
> **Prompt Eficaz:** "### Tarefa ### Resuma o texto fornecido abaixo sobre a história da computação. ### Instruções Adicionais ### 1. O resumo deve ter aproximadamente 300 palavras. 2. Foque nos marcos mais importantes. 3. O público-alvo são estudantes do ensino médio. 4. Apresente o resumo em três parágrafos concisos. 5. Evite jargões técnicos excessivos. ### Texto ### [COLE O TEXTO AQUI]".
*(Neste exemplo usamos: Controle de formato de saída, Restrições negativas, Definição de público e Delimitadores).*

**B. Geração de E-mails Profissionais**
> **Prompt Eficaz:** "### Tarefa ### Escrever um rascunho de e-mail. ### Contexto ### O cliente João Mendes teve seu pedido atrasado devido a um problema no fornecedor. ### Objetivo ### Pedir desculpas pelo inconveniente, mantê-lo informado e oferecer um desconto na próxima compra. Tom: Profissional, conciso e empático. ### Estrutura Sugerida ### 1. Saudação cordial. 2. Explicação do atraso. 3. Oferta do desconto. 4. Despedida.".
*(Neste exemplo usamos: Contexto claro, Estrutura de saída, Definição de tom de voz e Objetivo direto).*

**C. Geração de Ideias de Negócios (Brainstorming Assistido)**
> **Prompt Eficaz:** "Aja como um consultor de negócios especializado em tecnologia sustentável. Sou um engenheiro de software e tenho R$ 50.000 para investir. Sugira 3 ideias de negócios inovadoras para um aplicativo que combata o desperdício de alimentos no Brasil. Para cada ideia, descreva o problema, a solução, o público-alvo e o modelo de monetização. Apresente em formato de lista numerada. As ideias devem ser viáveis com o capital mencionado.".
*(Neste exemplo usamos: Role Prompting/Persona, Contexto do usuário, Restrições de viabilidade e Controle de formato de saída JSON/Lista).*

### Prompt Melhorado

## Crie um guia estruturado sobre Engenharia de Prompt contendo:

- Introdução histórica
- Fundamentos dos LLMs
- Técnicas de prompting
- Glossário
- Exemplos práticos
- Biblioteca de prompts reutilizáveis

## Resultado: O conteúdo passou a ter seções organizadas e melhor clareza. Observe abaixo:

Como engenheiro de prompt, estruturei este guia definitivo e avançado para você dominar a comunicação com as Inteligências Artificiais Generativas. 

### 1. Introdução Histórica
A busca humana pela comunicação com máquinas remonta aos autômatos mecânicos, mas ganhou base científica com o artigo de Alan Turing em 1950, que propôs o "Jogo da Imitação" (Teste de Turing). Nas décadas seguintes, o Processamento de Linguagem Natural (PLN) evoluiu através de sistemas baseados em regras rígidas, como o ELIZA (1960s), que simulava um psicoterapeuta reconhecendo palavras-chave. 

A verdadeira revolução ocorreu com o advento do Aprendizado de Máquina (Machine Learning) e as Redes Neurais Artificiais, permitindo que os computadores aprendessem padrões a partir de dados. O marco definitivo foi a introdução da **arquitetura Transformer** pelo Google em 2017, com o mecanismo de "auto-atenção" (self-attention), que permitiu aos modelos processar o contexto global de frases em paralelo. Isso pavimentou o caminho para os Grandes Modelos de Linguagem (LLMs), como o GPT-3 e o lançamento do ChatGPT em 2022, que democratizou a **Engenharia de Prompt**, transformando-a de uma arte intuitiva em uma disciplina essencial.

### 2. Fundamentos dos LLMs
Para criar comandos eficazes, é vital entender como a "mente" da máquina funciona:
*   **Mecanismo Probabilístico:** O ChatGPT não "pensa" de forma consciente; ele é um motor estatístico avançado projetado para calcular e prever o próximo *token* (palavra ou pedaço de palavra) mais provável em uma sequência.
*   **Pré-treinamento e RLHF:** A IA primeiro absorve vasto conhecimento da internet (Pré-treinamento) e, em seguida, é polida através do Aprendizado por Reforço com Feedback Humano (RLHF), que a ensina a seguir instruções, ser útil e segura.
*   **Janela de Contexto:** É a "memória de curto prazo" do modelo. Tudo que ultrapassa a janela de contexto (medida em tokens) é "esquecido" durante uma conversa, exigindo que você reafirme as regras para tarefas muito longas.

### 3. Técnicas de Prompting
Para extrair respostas de alto nível, aplicamos técnicas estratégicas:
*   **Zero-Shot e Few-Shot Prompting:** O *Zero-Shot* dá uma instrução direta sem exemplos prévios, ideal para tarefas simples. Já o *Few-Shot* fornece de 2 a 5 exemplos de como a entrada e a saída devem ser. A IA reconhece o padrão e o replica com altíssima precisão.
*   **Atribuição de Persona (Role Prompting):** Instruir a IA a agir como um especialista (ex: "Você é um consultor financeiro sênior"). Isso calibra instantaneamente o vocabulário, o tom e a profundidade analítica da resposta.
*   **Cadeia de Pensamento (Chain-of-Thought - CoT):** Exigir que a IA "pense passo a passo" ou mostre as etapas lógicas antes da resposta final. Isso força o modelo a decompor problemas matemáticos ou analíticos, reduzindo drasticamente erros de raciocínio.
*   **Restrições Negativas:** Estabelecer regras do que a IA **não** deve fazer (ex: "Não use jargões", "Não ultrapasse 100 palavras"). Isso delimita o escopo e evita divagações e alucinações.
*   **Decomposição de Tarefas:** Em vez de um "super prompt" para um projeto gigante, você divide a tarefa em blocos (ex: primeiro o esboço, depois a introdução), onde a saída de um prompt serve de entrada para o próximo.
*   **Árvore de Pensamentos (ToT):** Uma técnica avançada que instrui o modelo a gerar múltiplas rotas possíveis para a solução de um problema e avaliar os prós e contras de cada uma antes de decidir.

### 4. Glossário
*   **Token:** A unidade fundamental que a IA processa (pode ser uma palavra, uma sílaba ou até um caractere).
*   **Alucinação:** Quando a IA gera informações factualmente incorretas, enganosas ou fabricadas, mas as apresenta com extrema confiança.
*   **Temperatura:** Um parâmetro (geralmente de 0 a 2) que controla a aleatoriedade da IA. Temperaturas baixas (0.1 - 0.3) geram respostas focadas e factuais; temperaturas altas geram criatividade e diversidade.
*   **RLHF (Reinforcement Learning from Human Feedback):** O método usado para alinhar o comportamento do modelo às expectativas humanas, punindo respostas tóxicas e premiando respostas úteis.
*   **LLM (Large Language Model):** Um grande modelo de linguagem baseado em arquitetura Transformer, especializado em compreender e gerar linguagem natural.

### 5. Exemplos Práticos
Aqui está como a combinação de técnicas cria prompts robustos na vida real:

**Exemplo A: Geração de Ideias de Negócios (Uso de Persona + Restrições + Formato)**
> "Aja como um consultor de negócios especializado em startups de tecnologia sustentável. Sou um engenheiro de software com R$ 50.000 para investir e interesse em reduzir o desperdício de alimentos. Sugira 3 ideias de negócios inovadoras para um aplicativo no Brasil. Para cada ideia, descreva o problema, a solução, o público-alvo e o modelo de monetização. As ideias devem ser viáveis com o capital mencionado. Apresente em formato de lista numerada."

**Exemplo B: Resumo de Textos (Uso de Contexto + Público-alvo + Restrições Negativas)**
> "### Tarefa ### Resuma o texto fornecido abaixo sobre a Guerra Fria. ### Instruções ### 1. O resumo deve ter no máximo 5 parágrafos. 2. Foque nas causas e eventos principais. 3. O público-alvo são estudantes do ensino médio. 4. Evite jargões acadêmicos excessivos. ### Texto ### [COLE O TEXTO AQUI]."

### 6. Biblioteca de Prompts Reutilizáveis
Copie, cole e adapte os colchetes com os dados do seu negócio ou rotina:

*   **1. Desdobramento de Metas (Gestão de Projetos):**
    > "Você é um gerente de projetos experiente. Meu objetivo é [INSERIR OBJETIVO]. Minha equipe tem [NÚMERO] pessoas e usamos as ferramentas [LISTA DE FERRAMENTAS]. Quebre este objetivo em fases, tarefas semanais e ações diárias para os próximos 7 dias. Para cada tarefa, indique o responsável, prazo e prioridade. Forneça o resultado em formato Markdown ou Tabela."

*   **2. Extração de Ações de Reuniões (Produtividade):**
    > "Aqui está a transcrição de uma reunião: [COLAR TRANSCRIÇÃO]. Aja como um assistente executivo e extraia os 5 action items mais críticos. Para cada um, defina: o que fazer, quem é o responsável e qual é o prazo. Formate como lista de tarefas com checkboxes."

*   **3. Criação de E-mails Frios e de Vendas (Marketing):**
    > "Aja como um especialista em e-mail marketing. Escreva um e-mail para [NOME DO DESTINATÁRIO], que tem o cargo de [CARGO]. O objetivo do e-mail é [OBJETIVO, ex: agendar uma reunião de 15 minutos]. Destaque este benefício principal da nossa solução: [INSERIR BENEFÍCIO]. O tom deve ser profissional, empático e conciso. Não mencione custos nesta etapa."

*   **4. Tutor Particular para Assuntos Complexos (Estudos):**
    > "Aja como um professor paciente e didático. Explique o conceito de [CONCEITO COMPLEXO] para alguém que é [NÍVEL DE CONHECIMENTO, ex: leigo completo]. Use uma analogia simples do dia a dia para tornar a ideia clara. Divida a explicação em três partes e, ao final, faça uma pergunta para testar meu entendimento."

*   **5. O Método do "Pergunte ao Contrário" (Debate e Análise Crítica):**
    > "Eu defendo a tese de que [INSERIR TESE]. Aja como o 'advogado do diabo' e um crítico especializado neste mercado. Apresente os 3 contra-argumentos mais fortes e persuasivos contra a minha tese. Depois, sugira como eu poderia modificar minha tese original para me defender dessas objeções."


### Prompt Final Refinado

Crie um guia avançado e estruturado sobre Engenharia de Prompt contendo:

- Evolução histórica da IA
- Fundamentos técnicos (Transformers, Tokens, Embeddings)
- Técnicas avançadas (Zero-shot, Few-shot, Chain-of-Thought)
- Controle de qualidade (Temperatura, Alucinações)
- Glossário técnico
- Biblioteca prática de prompts reutilizáveis

Utilize linguagem técnica e estrutura profissional.

## Resultado: O resultado final gerou o documento "Guia Definitivo: Engenharia de Prompt e o Domínio das LLMs", utilizado como base do MiniGuia deste projeto.

Como engenheiro de prompt, estruturei este guia avançado para aprofundar sua compreensão técnica sobre a Inteligência Artificial Generativa. Este material vai desde a arquitetura fundamental dos modelos até a aplicação rigorosa de técnicas de controle e estruturação de comandos.

### 1. Evolução Histórica da IA
A busca pela comunicação com máquinas começou com conceitos teóricos, como o Teste de Turing em 1950, que propôs que uma máquina seria inteligente se suas respostas fossem indistinguíveis das humanas. O Processamento de Linguagem Natural (PLN) evoluiu inicialmente através de sistemas baseados em regras rígidas, como o ELIZA (década de 1960) e o SHRDLU, que operavam por reconhecimento de padrões e substituição de palavras-chave, mas falhavam em capturar a complexidade do contexto humano.

O verdadeiro salto ocorreu com o Aprendizado de Máquina (Machine Learning) e as Redes Neurais Artificiais (Deep Learning). Em vez de regras manuais, os algoritmos passaram a identificar padrões em vastos conjuntos de dados. A revolução definitiva para os Grandes Modelos de Linguagem (LLMs) foi a introdução da **arquitetura Transformer** em 2017, pelo Google, que abandonou o processamento sequencial das redes neurais anteriores em favor do processamento paralelo. Isso abriu caminho para modelos como a série GPT da OpenAI, culminando na democratização da engenharia de prompt.

### 2. Fundamentos Técnicos
Para dominar a engenharia de prompt, é crucial entender a "física" subjacente aos modelos:

*   **Tokens:** O texto do seu prompt não é lido como palavras inteiras, mas dividido em unidades menores chamadas tokens (que podem ser uma palavra, uma sílaba ou um caractere). Cada token é mapeado para um identificador numérico único. Entender a tokenização é vital, pois os modelos processam informações e são cobrados financeiramente com base na quantidade de tokens, possuindo limites estritos de "janela de contexto".
*   **Embeddings:** Os tokens numéricos são convertidos em representações vetoriais chamadas *word embeddings*. Esses vetores densos, em um espaço de alta dimensionalidade, capturam as relações semânticas e sintáticas entre as palavras. É por meio dos embeddings que o modelo "entende" que as palavras "rei" e "rainha" possuem relações similares a "homem" e "mulher".
*   **Transformers e Mecanismo de Auto-Atenção (Self-Attention):** A arquitetura Transformer processa os embeddings utilizando a auto-atenção. Isso significa que, para cada token gerado, o modelo "olha" para todos os outros tokens do prompt simultaneamente, calculando pesos matemáticos para determinar quais palavras são mais relevantes para o contexto.

### 3. Técnicas Avançadas de Prompting
O controle do espaço latente do modelo exige instruções arquitetadas cientificamente.

*   **Zero-Shot Prompting:** Consiste em dar uma instrução direta sem fornecer nenhum exemplo prévio. O modelo baseia-se puramente em seu treinamento massivo para generalizar e deduzir a resposta correta. É ideal para tarefas comuns, como traduções simples ou geração de listas.
*   **Few-Shot Prompting (Poucos Tiros):** Para saídas complexas que exigem um formato estrito ou tom específico, o prompt é enriquecido com exemplos de "entrada e saída". Ao fornecer 2 a 5 exemplos padronizados, o modelo reconhece a estrutura lógica (aprendizado em contexto) e a replica com altíssima precisão na nova requisição.
*   **Chain-of-Thought (Cadeia de Pensamento - CoT):** Técnica desenhada para resolver problemas de matemática, lógica ou planejamento. Em vez de pedir apenas a resposta final, o prompt instrui o modelo a "pensar passo a passo" ou "mostrar seu trabalho". A decomposição do problema obriga o modelo a alocar computação para cada etapa intermediária, reduzindo drasticamente os erros de salto lógico.

### 4. Controle de Qualidade
A previsibilidade do modelo é gerenciada pelo controle de seus parâmetros e delimitações estruturais.

*   **Temperatura (Temperature) e Top_p:** São parâmetros algorítmicos que controlam a aleatoriedade da geração de tokens. Uma temperatura baixa (ex: 0.1 - 0.2) gera respostas determinísticas, focadas e seguras, ideais para análise de dados e documentos legais. Uma temperatura alta (ex: 0.8 - 1.0) induz diversidade lexical, sendo ideal para escrita criativa e brainstorming.
*   **Mitigação de Alucinações:** Modelos preditivos podem gerar "alucinações" — informações factualmente falsas, citações inexistentes ou dados fabricados apresentados com grande confiança. Como engenheiro, você controla isso exigindo o *grounding* (ancoragem): instrua o modelo a responder *exclusivamente* com base no texto fornecido, exija que ele cite trechos exatos (com aspas) para justificar argumentos, ou dê a ele permissão explícita para dizer "Não sei" caso a informação não esteja nos dados.

### 5. Glossário Técnico
*   **LLM (Large Language Model):** Grandes modelos de linguagem baseados em Transformers, pré-treinados em bilhões de parâmetros para gerar texto.
*   **Janela de Contexto (Context Window):** A memória de curto prazo do modelo durante a inferência, medida em tokens. Se a conversa exceder esse limite, os dados mais antigos são esquecidos.
*   **RLHF (Reinforcement Learning from Human Feedback):** Técnica de aprendizado por reforço baseada em avaliação humana, usada para refinar o LLM e torná-lo útil, seguro e alinhado à intenção do usuário.
*   **Prompt Injection:** Uma vulnerabilidade de segurança onde comandos maliciosos contornam as diretrizes originais do sistema para forçar o modelo a executar ações indesejadas.
*   **Delimitadores:** Símbolos como `###`, `"""` ou `<tags> XML` usados visualmente e estruturalmente para separar regras, exemplos e dados de entrada bruto no prompt, evitando que a IA confunda as instruções.

### 6. Biblioteca Prática de Prompts Reutilizáveis
Estes templates utilizam as melhores práticas de delimitação, *few-shot*, contexto e atribuição de persona. Adapte as variáveis entre chaves `[ ]`.

**A. Geração de Ideias Estratégicas com Restrições (Brainstorming Técnico)**
> Aja como um consultor de negócios sênior especializado no setor de [INSERIR SETOR, ex: tecnologia sustentável].
> ### Contexto ###
> Sou um [INSERIR SUA PROFISSÃO] com interesse em atuar no problema de [INSERIR PROBLEMA]. Tenho um capital inicial de [INSERIR VALOR].
> ### Instrução Principal ###
> Sugira 3 ideias de negócios inovadoras para uma plataforma que resolva este problema.
> ### Restrições de Saída ###
> - As ideias devem ser estritamente viáveis com o capital mencionado.
> - Para cada ideia, defina: Nome provisório, O problema específico, A solução técnica, Público-alvo e Modelo de monetização.
> - Apresente o resultado em formato JSON.

**B. Resumo Extrativo com Grounding (Combate à Alucinação)**
> ### Tarefa ###
> Resumir o texto fornecido abaixo.
> ### Texto para Resumo ###
> """
> [INSERIR TEXTO BRUTO AQUI]
> """
> ### Instruções Adicionais ###
> 1. O resumo deve ter aproximadamente [INSERIR NÚMERO] palavras.
> 2. Foque exclusivamente nos marcos mais importantes apresentados no texto. Sob nenhuma hipótese invente dados externos.
> 3. O público-alvo são [INSERIR PÚBLICO, ex: estudantes universitários].
> 4. Apresente o resumo estruturado em formato de *bullet points* (marcadores).

**C. Assistente de Redação Formal (Ajuste de Tom e Objetivo)**
> ### Tarefa ###
> Escrever um e-mail profissional.
> ### Contexto ###
> Destinatário: [NOME DO CLIENTE]
> Motivo: [EXPLICAR O MOTIVO, ex: Atraso na entrega devido a problemas com o fornecedor]
> Objetivo: Pedir desculpas pelo inconveniente, informar a nova data e oferecer um desconto de [X]% na próxima compra.
> Tom: Profissional, conciso, empático e resolutivo.
> ### Instrução Principal ###
> Redija o e-mail utilizando as informações acima. Siga esta estrutura: Saudação cordial, Introdução do propósito, Destaque da solução/benefício, Agradecimento e Despedida.

---

> Este repositório documenta como usar engenharia de prompt com foco em maturidade técnica e automação estratégica para o dia a dia como parte do Bootcamp Accenture/DIO.

