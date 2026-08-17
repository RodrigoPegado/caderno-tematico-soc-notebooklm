# Mini Guia De Estudos
Abaixo está 5 mini guias sobre áreas relacionadas ao SOC.

# Security Operations Center (SOC)

Um Security Operations Center (SOC) é uma estrutura responsável por monitorar, detectar, investigar e responder a ameaças de segurança cibernética. Seu objetivo é proteger os sistemas e ativos de uma organização contra incidentes como malware, acessos não autorizados, vazamentos de dados e ataques de rede.

Um SOC pode ser mantido internamente pela organização ou terceirizado para um MSSP (Managed Security Services Provider).

Principais funções:
Monitoramento: acompanhamento contínuo de eventos e logs.

Detecção: identificação de comportamentos suspeitos e geração de alertas.

Triagem: análise dos alertas para determinar se representam uma ameaça real ou um falso positivo.

Resposta: contenção e remediação de incidentes.

Pós-incidente: documentação e análise das lições aprendidas.
Equipe

Os analistas geralmente são organizados em diferentes níveis:

N1: monitora alertas e realiza a triagem inicial.

N2: realiza investigações mais aprofundadas.

N3: atua em análises avançadas e casos complexos.

O funcionamento de um SOC depende do equilíbrio entre pessoas, processos e tecnologia. Pessoas qualificadas executam os processos de segurança utilizando ferramentas de monitoramento, detecção e investigação.

# NIST SP 800-61 — Resposta a Incidentes

O NIST SP 800-61 é um guia desenvolvido pelo National Institute of Standards and Technology (NIST) para auxiliar organizações a estruturar e melhorar seus processos de resposta a incidentes de segurança.

Seu objetivo é permitir que incidentes sejam tratados de maneira organizada e coordenada, reduzindo seus impactos e permitindo que a organização aprenda com os acontecimentos.

Ciclo de resposta a incidentes

O processo é dividido em quatro etapas principais:

Preparação: definição de políticas, procedimentos, responsabilidades, ferramentas e treinamento necessários para responder a incidentes.

Detecção e Análise: monitoramento do ambiente, identificação de possíveis incidentes e análise de alertas, logs e outras evidências para determinar se existe uma ameaça.
Contenção, Erradicação e Recuperação: após confirmar o incidente, a organização busca limitar sua propagação, remover a ameaça e restaurar os sistemas afetados.

Atividades Pós-Incidente: documentação do ocorrido, análise das causas e registro das lições aprendidas, permitindo melhorar os processos de segurança.
Relação com o SOC

O NIST SP 800-61 pode servir como uma estrutura para orientar o trabalho de um SOC durante a resposta a incidentes. Os analistas participam principalmente das atividades de monitoramento, detecção, análise e encaminhamento dos incidentes, enquanto equipes especializadas podem atuar nas etapas de contenção, erradicação e recuperação.

O framework também pode ser utilizado em conjunto com o MITRE ATT&CK, que ajuda a contextualizar as técnicas e comportamentos utilizados pelos atacantes.

# MITRE ATT&CK

O MITRE ATT&CK é uma base de conhecimento que organiza e documenta os comportamentos utilizados por adversários durante ataques cibernéticos. Ele fornece uma linguagem padronizada para que profissionais de segurança possam compreender, analisar e comunicar as ações realizadas por atacantes.

Táticas, técnicas e procedimentos:
O framework organiza os comportamentos dos atacantes em diferentes níveis:

Táticas: representam o objetivo do atacante, como obter acesso inicial, executar código, estabelecer persistência ou evitar mecanismos de defesa.

Técnicas: descrevem como o atacante busca alcançar esse objetivo.

Sub-técnicas: detalham métodos específicos utilizados dentro de uma técnica.

Procedimentos: representam exemplos de como determinada técnica foi utilizada na prática.

Por exemplo, um atacante pode utilizar phishing para conseguir acesso inicial a uma organização.

Uso no SOC

O MITRE ATT&CK pode auxiliar um SOC a:

Contextualizar alertas e compreender o comportamento do atacante;

Criar e aprimorar regras de detecção baseadas em técnicas conhecidas;

Identificar lacunas de segurança e pontos que precisam de melhorias;

Padronizar a comunicação entre profissionais de segurança;

Apoiar a investigação e resposta a incidentes.

Relação com detecção e resposta

Na detecção, o SOC pode utilizar as técnicas do ATT&CK para desenvolver mecanismos capazes de identificar comportamentos suspeitos.

# Triagem de Alertas no SOC

A triagem de alertas é o processo realizado pelo analista de SOC para analisar, validar e classificar alertas de segurança, determinando se representam uma atividade legítima ou um possível incidente.

Geração do alerta

Os alertas são gerados a partir de logs e eventos coletados de sistemas e dispositivos da organização. Ferramentas como SIEM, EDR e IDS analisam esses eventos e identificam comportamentos que podem indicar uma ameaça.

# Análise do alerta

Durante a investigação, o analista busca entender o que aconteceu, quais sistemas foram envolvidos e se existe atividade maliciosa. Para isso, pode analisar:

Dados de rede: IPs, portas, conexões e tráfego;

Logs de sistemas: processos, eventos e atividades realizadas;

Indicadores de Comprometimento (IoCs): hashes, IPs e domínios suspeitos;

Linha do tempo: sequência dos eventos relacionados ao alerta.

Ferramentas como Wireshark, Zeek, Sysmon e Windows Event Viewer podem auxiliar nessa análise.

Falso positivo e verdadeiro positivo

Após investigar o alerta, o analista precisa determinar sua natureza:

Falso positivo: uma atividade legítima foi identificada incorretamente como suspeita.

Verdadeiro positivo: a investigação confirmou uma atividade maliciosa ou não autorizada.

A identificação correta evita a fadiga de alertas, causada pelo excesso de notificações sem relevância.

Logs, Threat Intelligence e MITRE ATT&CK

Durante a investigação, diferentes fontes podem ser utilizadas:

Logs: ajudam a reconstruir a sequência dos acontecimentos;
Threat Intelligence: permite verificar a reputação de IPs, domínios e hashes suspeitos;
MITRE ATT&CK: ajuda a identificar e contextualizar as táticas e técnicas utilizadas pelo atacante.

Por exemplo, a identificação da técnica Scheduled Task/Job — T1053.005 pode indicar uma tentativa de estabelecer persistência.

Escalonamento

Quando o analista N1 identifica uma ameaça complexa ou que exige conhecimentos mais avançados, o alerta pode ser escalado para profissionais de N2, N3 ou para a equipe de resposta a incidentes (IRT).

O N1 deve registrar as evidências encontradas e documentar a investigação antes do escalonamento.

O conteúdo estudado mostra como os principais conceitos de Cibersegurança se conectam dentro de um SOC.

Conceitos principais
SOC: monitora, detecta, investiga e responde a ameaças.
Tríade CIA: Confidencialidade, Integridade e Disponibilidade.
IAAA: Identificação, Autenticação, Autorização e Auditoria.
NIST SP 800-61: orienta o processo de resposta a incidentes.
MITRE ATT&CK: organiza as táticas e técnicas utilizadas por atacantes.
Logs: registram atividades e fornecem evidências para investigação.
Como tudo se conecta

Logs → SIEM/EDR → Alerta → Analista N1 → Triagem → Investigação → Resposta

O MITRE ATT&CK ajuda a entender o comportamento do atacante, enquanto o NIST orienta como responder ao incidente.

Termos importantes

SIEM: centraliza e analisa logs.
EDR: monitora e responde a ameaças em endpoints.
SOAR: automatiza tarefas de segurança.
IoCs: evidências de possível comprometimento.
TTPs: comportamentos utilizados pelos atacantes.
MSSP: empresa que fornece serviços de segurança terceirizados.

# Glossário

SOC (Security Operations Center): equipe responsável por monitorar, detectar, investigar e responder a ameaças de segurança.

SIEM (Security Information and Event Management): plataforma que centraliza, correlaciona e analisa logs e eventos de segurança.

EDR (Endpoint Detection and Response): solução que monitora computadores e servidores em busca de atividades suspeitas.

IDS (Intrusion Detection System): sistema responsável por detectar possíveis atividades maliciosas em uma rede.

Log: registro de uma atividade ou evento ocorrido em um sistema, aplicação, rede ou dispositivo.

IoC (Indicator of Compromise): indicador que pode fornecer evidências de comprometimento, como um IP, domínio ou hash malicioso.

Threat Intelligence: informações utilizadas para compreender ameaças e avaliar indicadores relacionados a possíveis ataques.

MITRE ATT&CK: framework que organiza e documenta comportamentos, táticas e técnicas utilizados por atacantes.

TTP: sigla para Táticas, Técnicas e Procedimentos, utilizada para descrever o comportamento de ameaças.

N1: nível inicial de atuação do SOC, responsável principalmente pelo monitoramento e triagem dos alertas.

N2/N3: níveis mais especializados, responsáveis por investigações e incidentes de maior complexidade.

Falso Positivo: alerta identificado como suspeito, mas que posteriormente é confirmado como uma atividade legítima.

Verdadeiro Positivo: alerta que, após investigação, é confirmado como uma atividade realmente maliciosa.

Fadiga de Alertas: sobrecarga causada pelo grande volume de alertas recebidos pelos analistas.

NIST SP 800-61: publicação que apresenta orientações para preparação, detecção, análise e resposta a incidentes.

Tática: objetivo que um atacante busca alcançar dentro do MITRE ATT&CK.

Técnica: método utilizado pelo atacante para alcançar determinado objetivo.

MSSP: provedor externo que oferece serviços gerenciados de segurança para organizações.

SOAR: tecnologia utilizada para integrar ferramentas de segurança e automatizar processos de resposta.

# Prompts Reutilizáveis

Os prompts abaixo foram desenvolvidos para que possam ser reutilizados em diferentes conteúdos de Cibersegurança, permitindo que a IA Generativa atue como ferramenta de apoio ao aprendizado.

1. Explicar um conceito

Atue como um professor de Cibersegurança. Explique o conceito de [CONCEITO] de forma clara e didática para alguém com nível [NÍVEL]. Apresente a definição, explique como funciona, dê um exemplo prático e mostre sua relação com a atuação de um SOC.

2. Resumir um conteúdo

Resuma o conteúdo abaixo mantendo apenas as informações mais importantes para compreender [TEMA]. Organize em tópicos, destaque os conceitos fundamentais e utilize uma linguagem simples, sem perder a precisão técnica.

3. Analisar um alerta de SOC

Atue como um analista de SOC N1. Analise o seguinte alerta: [ALERTA]. Identifique os principais indicadores, explique o que pode ter acontecido, classifique possíveis hipóteses e indique quais informações adicionais deveriam ser investigadas antes de concluir se é um falso positivo ou um incidente real.

4. Relacionar com MITRE ATT&CK

Analise a atividade descrita abaixo e identifique quais possíveis táticas e técnicas do MITRE ATT&CK estão relacionadas. Explique o motivo de cada associação e diferencie claramente a tática da técnica. Atividade: [ATIVIDADE].

5. Criar questões para estudar

Crie [QUANTIDADE] questões sobre [TEMA] para testar meu conhecimento. Misture questões de múltipla escolha e questões abertas. Não apresente as respostas inicialmente. Depois que eu responder, corrija minhas respostas e explique meus erros.

6. Criar um cenário prático

Crie um cenário fictício de incidente de segurança envolvendo [TEMA]. Apresente o cenário como uma situação encontrada por um analista de SOC. Depois, peça para eu investigar o caso passo a passo, fornecendo novas informações conforme eu fizer perguntas ou tomar decisões.

7. Revisar meu conhecimento

Atue como um professor de Cibersegurança. Faça uma avaliação do meu conhecimento sobre [TEMA]. Comece com perguntas básicas e aumente gradualmente a dificuldade. Após cada resposta, explique o que acertei, o que errei e qual conceito devo revisar.
