
# Engenharia de prompts

# Prompt 1 - Contexto e Objetivos
Prompt: Analise todas as fontes adicionadas a este notebook e explique, de forma clara e organizada, o contexto do tema abordado e quais são os principais objetivos que podem ser definidos para um projeto sobre esse assunto.

Não invente informações que não estejam nas fontes. Sempre indique quais fontes sustentam cada informação.

Organize a resposta em:

Contexto do problema/tema

Por que esse tema é relevante

Problema que o projeto pretende abordar

Objetivo geral

Possíveis objetivos específicos

Objetivo: Identificar, a partir das fontes selecionadas, o contexto do tema, sua relevância, os principais problemas relacionados e possíveis objetivos para orientar o projeto.

Resultado obtido: O NotebookLM identificou que o tema está relacionado ao funcionamento de Security Operations Centers (SOC) e à gestão e resposta a incidentes de segurança. As fontes destacaram a importância de frameworks como NIST SP 800-61 e MITRE ATT&CK, além de problemas como fadiga de alertas, falsos positivos e necessidade de processos estruturados de resposta.

Como o resultado foi utilizado: As informações foram utilizadas para construir a seção "Contexto e Objetivos" do projeto, ajudando a definir o problema abordado, a relevância do tema, o objetivo geral e os objetivos específicos.

Avaliação: O prompt apresentou um resultado satisfatório, pois conseguiu organizar as informações das fontes de acordo com os tópicos solicitados. A resposta foi utilizada como base para a elaboração do contexto e dos objetivos do projeto, sendo posteriormente sintetizada e adaptada para o README.

# Prompt 2 - Aplicação de IA Generativa em SOC
Prompt: Com base exclusivamente nas fontes deste notebook, identifique como a Inteligência Artificial Generativa pode ser aplicada para auxiliar um analista de SOC nas atividades de detecção, triagem, análise e resposta a incidentes.

Considere especialmente a integração com o NIST SP 800-61 e o MITRE ATT&CK.

Apresente exemplos práticos de utilização de IA Generativa em cada etapa e destaque quais tarefas poderiam ser automatizadas ou apoiadas pela IA e quais ainda deveriam depender da decisão humana.

Não invente informações que não estejam sustentadas pelas fontes.

Objetivo: Verificar se as fontes selecionadas apresentavam informações suficientes para fundamentar aplicações de Inteligência Artificial Generativa no trabalho de um analista de SOC, identificando também quais atividades poderiam receber apoio de tecnologias de IA e quais dependem da atuação humana.

Resultado Obtido: O NotebookLM informou que as fontes não apresentavam informações diretamente relacionadas à aplicação de Inteligência Artificial Generativa no cotidiano de um analista de SOC. Entretanto, foram encontradas informações relacionadas ao uso de automação, Machine Learning e ferramentas SOAR para apoiar atividades de detecção e resposta a incidentes.

Como o resultado foi utilizado: O resultado permitiu identificar uma limitação das fontes selecionadas. Em vez de atribuir às fontes informações que elas não apresentavam, os conceitos encontrados sobre automação, Machine Learning, SOAR, NIST SP 800-61 e MITRE ATT&CK foram utilizados como base para compreender o contexto no qual uma solução de IA Generativa poderia ser proposta.

Avaliação: O prompt não atingiu completamente o objetivo inicial, pois as fontes não continham informações específicas sobre IA Generativa aplicada a SOC. Apesar disso, o resultado foi importante para identificar essa limitação e direcionar a pesquisa para informações que realmente estavam presentes nas fontes. Esse processo também demonstrou a necessidade de reformular os prompts quando as fontes disponíveis não são suficientes para responder à pergunta inicial.

# Prompt 3 - Processo de Triagem De Alertas
Prompt: Com base nas fontes deste notebook, descreva como poderia ser estruturado um processo de triagem e análise de um alerta de segurança em um SOC, desde o recebimento do alerta até a tomada de decisão pelo analista.

Identifique quais informações são analisadas, quais etapas fazem parte do processo e quais decisões precisam ser tomadas pelo analista.

Organize a resposta pensando na criação de um protótipo de assistente de IA Generativa para apoiar esse processo.

Objetivo: Compreender as principais etapas envolvidas na triagem e análise de um alerta de segurança e identificar de que forma um assistente de IA Generativa poderia apoiar o analista durante esse processo.

Resultado Obtido: O NotebookLM estruturou o processo em etapas que envolvem a coleta e análise de alertas, logs e outras evidências, contextualização das ameaças utilizando o MITRE ATT&CK, sugestão de ações de resposta e geração de documentação. A resposta também destacou a necessidade de manter uma divisão clara entre as atividades de apoio da IA e as decisões que devem permanecer sob responsabilidade do analista humano.

Como o resultado foi utilizado: O resultado foi utilizado para definir a proposta de funcionamento do projeto e estabelecer quais atividades poderiam ser realizadas pelo assistente de IA Generativa e quais continuariam dependendo da validação e decisão do analista de SOC.

Avaliação: O prompt apresentou um resultado satisfatório, pois conseguiu transformar os conceitos encontrados nas fontes em um fluxo de trabalho mais concreto. A resposta ajudou a definir o escopo do projeto e a estabelecer a IA como uma ferramenta de apoio à análise, e não como substituta do analista.
