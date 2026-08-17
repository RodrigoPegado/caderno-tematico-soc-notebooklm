
# Descrição da Soluçao
O SOC AI Assistant é um protótipo de assistente baseado em Inteligência Artificial Generativa desenvolvido para auxiliar analistas de Security Operations Center (SOC) durante a triagem e análise inicial de incidentes de segurança.

A solução recebe informações relacionadas a um alerta de segurança e utiliza IA Generativa para organizar e interpretar os dados, fornecendo ao analista uma visão estruturada do possível incidente.

O assistente não tem como objetivo substituir o profissional de segurança. Sua função é reduzir o trabalho manual, organizar informações e fornecer apoio à análise, enquanto a validação e a tomada de decisão permanecem sob responsabilidade do analista.

# Funcionamento Proposto
# Entrada das informações:
Descrição do alerta;

Logs e eventos relevantes;

Endereço IP ou domínio;

Usuário envolvido;

Horário dos eventos;

Processos ou arquivos suspeitos;

Indicadores de comprometimento (IoCs);

Outras evidências relacionadas ao incidente.

# Análise pela IA
A IA Generativa analisa as informações fornecidas e organiza os dados para facilitar a compreensão do incidente.

Resumo do possível incidente;

Evidências relevantes;

Possíveis causas ou comportamentos suspeitos;

Nível de severidade sugerido;

Possíveis técnicas e táticas relacionadas ao MITRE ATT&CK;

Pontos que precisam ser investigados pelo analista.

# Recomendações de Investigação
Com base nas informações analisadas, o assistente poderá sugerir perguntas e etapas para auxiliar a investigação.

Verificar outros eventos relacionados ao mesmo endereço IP;

Verificar atividades realizadas pelo usuário;

Investigar processos executados no equipamento;

Verificar se outros dispositivos apresentaram comportamento semelhante;

Buscar evidências adicionais antes de confirmar o incidente.

# Apoio á resposta
Após a análise, o assistente poderá apresentar possíveis ações de resposta e contenção relacionadas ao cenário identificado.

O analista será responsável por avaliar o contexto e decidir quais medidas devem ser tomadas.

# Geração de Relatório
Um dos princípios do projeto é manter uma divisão clara entre o auxílio fornecido pela IA e a responsabilidade do profissional de segurança.

| IA Generativa                   | Analista de SOC                     |
| ------------------------------- | ----------------------------------- |
| Organiza as informações         | Valida as informações               |
| Resume os eventos               | Analisa o contexto                  |
| Sugere possíveis classificações | Decide a classificação final        |
| Sugere técnicas MITRE ATT&CK    | Valida o mapeamento                 |
| Sugere etapas de investigação   | Decide quais investigações realizar |
| Sugere ações de resposta        | Autoriza e executa as ações         |
| Gera um relatório preliminar    | Revisa e aprova o relatório         |

Dessa forma, o SOC AI Assistant atua como uma ferramenta de apoio à decisão, e não como um sistema autônomo de resposta a incidentes.
