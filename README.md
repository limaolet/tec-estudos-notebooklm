# tec-estudos-notebooklm
Este documento descreve os fundamentos técnicos dos Modelos de Linguagem de Grande Porte (LLMs), categoriza os riscos operacionais de acordo com os marcos regulatórios brasileiros emergentes e estabelece uma diretriz clara para o setor público: a supervisão humana é inegociável. A implementação eficaz requer uma transição do mero uso para a "Alfabetização em IA", garantindo que os servidores públicos possam avaliar criticamente os resultados, respeitando os princípios administrativos fundamentais de legalidade, impessoalidade, moralidade, publicidade e eficiência.

1. Contexto e Objetivos
O assunto escolhido para este caderno é a fundamentação técnica e as diretrizes éticas para o uso de Inteligência Artificial Generativa. O objetivo de estudo é capacitar o usuário a compreender como os Grandes Modelos de Linguagem (LLMs) funcionam, identificar os riscos inerentes (como alucinações e vieses) e aplicar as recomendações de segurança e governança estabelecidas para o serviço público brasileiro.

--------------------------------------------------------------------------------

2. Curadoria de Fontes
As fontes utilizadas para esta análise e inseridas no NotebookLM são:
Fonte 1: Cartilha IA Generativa — Governo Digital (Ministério da Gestão e da Inovação/SERPRO).

Fonte 2: O que é Inteligência Artificial? (Microsoft Azure).

Fonte 3: What are large language models (LLMs)? (Microsoft Azure).

--------------------------------------------------------------------------------

3. Engenharia de Prompts e "Cicatrizes"
Para extrair o melhor conteúdo das fontes, foram testadas diferentes estratégias de interação:

Pergunta Estratégica 1: "Diferencie IA Analítica de IA Generativa."
Resposta obtida: A analítica foca em previsões e classificações de dados existentes; a generativa cria conteúdo novo (sintético).

Dificuldade: Inicialmente, a resposta foi genérica. Foi necessário ajustar o prompt para: "Explique a diferença com foco nos objetivos de cada uma conforme a Cartilha do Governo Digital" para obter a distinção entre suporte à decisão e criação de conteúdo.

Pergunta Estratégica 2: "Quais são os riscos de segurança no uso de LLMs externos?"
Resposta obtida: Vazamento de dados sensíveis, exposição de credenciais e falta de transparência ("caixas-pretas").

Cicatriz/Lição: O modelo por vezes ignorava a distinção entre ferramentas internas e externas. O prompt foi refinado para "Liste os riscos específicos de ferramentas comerciais como ChatGPT comparadas a soluções internas aprovadas".

Pergunta Estratégica 3: "Como funciona tecnicamente um LLM?"
Resposta obtida: Uso de arquitetura Transformer, processamento de tokens e cálculo de probabilidades estatísticas para prever a próxima palavra.

Troubleshooting: O termo "alucinação" apareceu como um erro humano em tentativas falhas. O ajuste no prompt solicitou a "definição técnica de alucinação baseada na arquitetura probabilística" para esclarecer que é um subproduto da falta de compreensão real de contexto.

--------------------------------------------------------------------------------

4. Miniguia de Estudo (Entrega Final)
A. Resumos Estruturados
Funcionamento Técnico: A IA imita funções cognitivas humanas através de matemática e lógica.
Os LLMs utilizam redes neurais profundas (Transformers) para processar sequências de texto, dividindo-os em tokens e convertendo-os em embeddings (representações numéricas) para capturar significado e contexto.

Classificação de Riscos (PL 2338/2023):
Risco Excessivo: Sistemas proibidos, como pontuação social ou manipulação de grupos vulneráveis.
Alto Risco: Sistemas que exigem governança rigorosa, como os usados em saúde, segurança e identificação biométrica.
Risco Moderado/Baixo: Exigem transparência e boas práticas, como chatbots de atendimento e filtros de recomendação.

Diretrizes para Servidores: A revisão humana é inegociável; o servidor é o responsável final pelo conteúdo. 
Deve-se priorizar ferramentas internas aprovadas e nunca inserir dados sigilosos em modelos públicos.

B. Glossário de Conceitos Chave
IA Generativa (IAG): IA focada na criação de novos conteúdos (texto, imagem, código).
LLM (Large Language Model): Modelos de linguagem treinados em vastos conjuntos de dados para entender e gerar texto natural.
Alucinação: Geração de informações factualmente incorretas, mas convincentes, devido a limites na arquitetura probabilística.
Prompt: Comando ou instrução fornecida pelo usuário para orientar a resposta da IA.
RAG (Geração Aumentada via Recuperação): Técnica que combina o modelo de IA com uma base de dados externa específica para fornecer respostas mais precisas e atualizadas.
Token: Menor unidade de texto (palavra ou caractere) que o modelo processa.
Vieses: Tendências ou preconceitos presentes nos dados de treinamento que a IA pode replicar.

C. Prompts Reutilizáveis para Revisão
"Resuma os princípios éticos da Moralidade e Impessoalidade aplicados ao uso de IA no setor público conforme as fontes."
"Explique a importância da anonimização de dados antes de utilizar ferramentas de IA generativa."
"Quais são as 'Boas Práticas' recomendadas para a Elaboração e Revisão de Documentos oficiais com auxílio de IA?"
"Compare as vantagens e desafios dos modelos abertos versus modelos fechados de IA."
