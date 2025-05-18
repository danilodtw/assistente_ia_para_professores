Assistente de IA para Professores

Uma Ferramenta para Otimizar o Planejamento e a Avaliação Educacional
Este projeto MVP (Produto Mínimo Viável) demonstra a criação de um assistente inteligente baseado em Inteligência Artificial para auxiliar educadores em tarefas comuns do dia a dia. O objetivo principal é reduzir a carga de trabalho manual e permitir que os professores dediquem mais tempo à interação com os alunos e à personalização do ensino.

Desenvolvido como parte da Imersão IA da Alura com o Google, este projeto utiliza as ferramentas e conceitos abordados no treinamento para criar um sistema prático e com potencial de impacto na área da educação.
Funcionalidades Implementadas (MVP)
Atualmente, o assistente oferece as seguintes funcionalidades básicas:
 - Criação de Aulas e Conteúdo:
   - Recebe o tópico, série/nível e objetivos de aprendizagem.
   - Utiliza um agente especializado (agente_planejador_aula) para gerar uma estrutura de plano de aula detalhada.
   - Utiliza outro agente (agente_gerador_conteudo) para gerar um rascunho do conteúdo da aula com base no plano.
   - Ambos os agentes utilizam a ferramenta Google Search para buscar informações e recursos relevantes.

 - Preparação de Provas e Avaliações:
   - Recebe o tópico, série/nível, tipo de questão, nível de dificuldade e número de questões desejado.
   - Utiliza um agente especializado (agente_gerador_questoes) para gerar um conjunto de questões relevantes.
   - Gera um modelo de cartão resposta textual no formato compatível com a funcionalidade de correção futura.
   - O agente utiliza a ferramenta Google Search para buscar informações relevantes para a criação das questões.

 - Correção de Provas e Avaliações (Estrutura Inicial):
   - Possui a estrutura para receber o texto da prova, gabarito/critérios e respostas do aluno em um formato textual estruturado.
   - Utiliza um agente (agente_corretor_provas) para processar a entrada e gerar um resultado de correção básico.
   - Nota: A correção de questões dissertativas é complexa e requer refinamento extensivo do prompt no Google AI Studio.

 - Tecnologias e Ferramentas Utilizadas
   - Google Colab: Ambiente principal para desenvolvimento e execução do código Python.
   - Google AI Studio: Ferramenta fundamental para prototipar, testar e refinar as instruções (prompts) que guiam o comportamento dos agentes.
   - Google Gemini: O modelo de linguagem poderoso que serve como o "cérebro" dos agentes, responsável pela geração de texto, compreensão e análise. Utilizamos o modelo gemini-2.0-flash.
   - Google Agent Developer Kit (ADK): Framework utilizado para definir e orquestrar os diferentes agentes especializados que compõem o assistente.
   - Google Search Tool: Ferramenta integrada aos agentes criativos para permitir a busca por informações atualizadas na web.

 - Como Usar (MVP no Google Colab)
   - Clone o Repositório: Faça o download ou clone este repositório para o seu ambiente.
   - Abra no Google Colab: Carregue o arquivo .ipynb (ou copie o código Python) em um novo notebook do Google Colab.
   - Configure sua API Key:
       - Obtenha sua API Key do Google Gemini.
       - No Google Colab, vá para o menu lateral esquerdo, clique no ícone de chave (🔑 Segredos).
       - Clique em + Novo segredo e adicione um segredo com o nome GOOGLE_API_KEY e o valor da sua chave.
   - Execute o Notebook: Rode todas as células do notebook.
   - Interaja com o Menu: Siga as instruções no console para escolher uma das funcionalidades implementadas e fornecer os inputs necessários.

 - Potencial e Próximos Passos
   - Este MVP é apenas o começo. O projeto tem um grande potencial para se tornar uma ferramenta poderosa para educadores. Os próximos passos incluem:
       - Completar a implementação da funcionalidade "Preparar Provas e Avaliações" (incluindo diferentes formatos de prova).
       - Desenvolver a funcionalidade "Corrigir Provas e Avaliações", focando inicialmente em correção de múltipla escolha e, posteriormente, explorando a correção de dissertativas com refinamento avançado no Google AI Studio.
       - Implementar a leitura de cartões resposta digitalizados em PDF (funcionalidade avançada que envolveria processamento de imagem e OCR - registrado como TODO no código).
       - Melhorar a interface do usuário (considerar o uso de frameworks como Streamlit para uma interface web mais amigável).
       - Integrar com Google Drive ou outras plataformas para facilitar o upload/download de materiais.
       - Adicionar mais tipos de agentes especializados (ex: agente para gerar atividades práticas, agente para criar rubricas de avaliação).

Sinta-se à vontade para explorar o código, testar as funcionalidades e contribuir com ideias para o futuro do projeto!
